# Divisiones Políticas Departamental y Municipal en Colombia 
Creado con información publica en la [Geopartal DANE de Colombia](https://geoportal.dane.gov.co/servicios/descarga-y-metadatos/descarga-mgn-marco-geoestadistico-nacional/). Allí puedes obtener las divisiones políticas [municipales]('https://geoportal.dane.gov.co/descargas/mgn_2018/MGN2018_MPIO_POLITICO.rar') y [departamentales]('https://geoportal.dane.gov.co/descargas/mgn_2018/MGN2018_DPTO_POLITICO.zip') en formato *shape* .shp. 

Con la aplicación [mapshaper.org](https://mapshaper.org/) de [Matt Bloch](http://www.cartogis.org/docs/proceedings/2006/bloch_harrower.pdf) los detalles geográficos fueron simplificados y exportados a formato topojson, creando un archivo mas liviano.

Después el topojson fue convertido a dos archivos geojson (municipal y departamental) con la biblioteca [topo2geo](https://github.com/kylepollina/topo2geo). 

Estos archivos geojson son útil para crear mapas [coropletas con plotly](https://plotly.com/python/choropleth-maps/).

Nota: si es posible convertir de .shp directamente a geojson con [mapshaper.org](https://mapshaper.org/) pero este geojson no dio resultado en ploty.
