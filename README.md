# Robot de estadísticas de ArgentinaCS

Consulta GameTracker cada 10 minutos y publica en la rama `datos` un archivo
`todos.json` con el estado de los 26 servidores de Counter-Strike 1.6:
jugadores conectados, mapa actual, ranking y top 10.

El sitio [argentinacs.com.ar](https://argentinacs.com.ar) lo lee desde ahí para
mostrar el detalle de cada servidor.

**Por qué está separado del repo del sitio:** al correr cada 10 minutos genera
muchas ejecuciones, y mezclarlo con el repositorio del sitio ensuciaba el
historial de despliegues. Acá vive solo y no molesta a nadie.

Para cambiar la lista de servidores: editar `tools/servers.tsv`.
