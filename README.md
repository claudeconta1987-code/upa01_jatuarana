# UPA 01 · UMF I · FLONA Jatuarana: mapa para desenho de estradas

Mapa interativo (arquivo único, `index.html`) com árvores de corte, filtro de espécies, APPs, UTs, SRTM e ferramenta de desenho de traçado com corredor de 300 m e volume por espécie.

## Publicar no GitHub Pages
1. Crie um repositório e envie `index.html` e este `README.md` para a raiz.
2. Em **Settings → Pages**: *Source* = *Deploy from a branch*, *Branch* = `main`, pasta `/ (root)`.
3. O endereço sai em `https://<usuario>.github.io/<repositorio>/`.

## Observações
- Tudo roda no navegador; os traços desenhados ficam salvos no próprio navegador (localStorage) e podem ser exportados em GeoJSON/KML.
- Fundos Satélite/Mapa precisam de internet; SRTM e "Sem fundo" funcionam offline.
- Atenção: a página contém coordenadas, espécie e volume de cada árvore do inventário. GitHub Pages é público.
