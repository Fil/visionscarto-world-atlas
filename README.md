## Natural Earth vector data, fixed & packaged

- fixes topological issues on the border of Sudan
- uses UN definition for Morrocco / Western Sahara
- adds a few Kuril Islands
- adds Gaza
- keeps all properties fields from NE
- also export countries and land in GeoJSON

## Usage

You can use this as a drop-in replacement for [world-atlas](https://github.com/topojson/world-atlas) data:

In TopoJSON:
```{javascript}
fetch('https://unpkg.com/ne110m_fixes/world/110m.json').then(d => d.json())
```

In GeoJSON:
```{javascript}
fetch('https://unpkg.com/ne110m_fixes/world/110m_land.geojson').then(d => d.json())
```

With d3:
In GeoJSON:
```{javascript}
d3.json('https://unpkg.com/ne110m_fixes/world/50m_countries.geojson')
```

…

## Credits

The hard work has been done by the team
at [Natural Earth](https://www.naturalearthdata.com/).

Mike Bostock has contributed all the necessary tooling
and examples in [world-atlas](https://github.com/topojson/world-atlas).
