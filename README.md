# Mapa Espinosa

Site estático para consultar as coordenadas de um arquivo KML e abrir cada ponto no Google Earth Web.

## Publicar o mapa

Coloque o arquivo `Comunidades Rurais.kml` na raiz do site, ao lado de `index.html`. O navegador lê esse arquivo hospedado, então todos os visitantes veem o mesmo mapa. O KML não é enviado a um servidor por um formulário.

Para testar localmente, sirva a pasta por HTTP, por exemplo com `python3 -m http.server 8000`, e abra `http://localhost:8000`.

## Google Earth Web

A lista paginada abre cada coordenada no Google Earth Web. A aba “Projeto Earth” abre o projeto compartilhado [Comunidades Rurais](https://earth.google.com/earth/d/1WiYrq9xgROuRRJoFwIrFEnfGo77ttYg_?usp=sharing). O Google Earth envia `X-Frame-Options: SAMEORIGIN`, então não permite exibir esse projeto dentro de um `iframe` hospedado em outro site.
