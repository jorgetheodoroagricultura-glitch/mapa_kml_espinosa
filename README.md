# Mapa Espinosa

Site estático para consultar coordenadas, visualizar as geometrias do KML em um globo Cesium incorporado e abrir o projeto no Google Earth Web.

Publicado em: https://jorgetheodoroagricultura-glitch.github.io/mapa_kml_espinosa/ . Atualizações em `main` são publicadas automaticamente pelo GitHub Actions.

## Publicar o mapa

Coloque o arquivo `Comunidades Rurais.kml` na raiz do site, ao lado de `index.html`. O navegador lê esse arquivo hospedado, então todos os visitantes veem o mesmo mapa. O KML não é enviado a um servidor por um formulário.

Para testar localmente, sirva a pasta por HTTP, por exemplo com `python3 -m http.server 8000`, e abra `http://localhost:8000`.

## Google Earth Web

A lista paginada abre cada coordenada no Google Earth Web. A aba “Projeto Earth” incorpora um globo Cesium com as geometrias do KML; o botão da aba também abre o projeto compartilhado [Comunidades Rurais](https://earth.google.com/earth/d/1WiYrq9xgROuRRJoFwIrFEnfGo77ttYg_?usp=sharing). O projeto original não pode ser incorporado diretamente porque o Google Earth envia `X-Frame-Options: SAMEORIGIN`.
