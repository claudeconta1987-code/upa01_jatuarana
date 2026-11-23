# UPA 01 · UMF I · FLONA Jatuarana: mapa para desenho de estradas

Mapa interativo (arquivo único, `index.html`) com árvores de corte e remanescentes 2 (estrela, só visualização), filtro de espécies e por nome comercial/vulgar, APPs, UTs, SRTM e ferramenta de desenho de traçado com corredor de 300 m e volume por espécie.

## Publicar no GitHub Pages
1. Crie um repositório e envie `index.html` e este `README.md` para a raiz.
2. Em **Settings → Pages**: *Source* = *Deploy from a branch*, *Branch* = `main`, pasta `/ (root)`.
3. O endereço sai em `https://<usuario>.github.io/<repositorio>/`.

## Observações
- Tudo roda no navegador; os traços desenhados ficam salvos no próprio navegador (localStorage) e podem ser exportados em GeoJSON/KML.
- Fundos Satélite/Mapa precisam de internet; SRTM e "Sem fundo" funcionam offline.
- Atenção: a página contém coordenadas, espécie e volume de cada árvore do inventário. GitHub Pages é público.

## Lista completa

`arvores_corte_remanescente2_upa01.xlsx`: todas as árvores de corte e remanescente 2 do inventário (consolidado V3AM), com filtro por nome comercial e nome vulgar. Link de download no painel "Árvores" do mapa.

## Projeção de remanescentes (juntar UTs)

Painel "Projeção de remanescentes": marque UTs (ou digite `1-4, 7`) para tratá-las como uma só unidade de manejo. A regra é a da planilha (R2 por UT + espécie) aplicada à junta: densidade = indivíduos acima do DMC ÷ área sem APP; "Pouco abundante"/"Rara" retêm todas; "Normal" retém o maior entre % mínimo × indivíduos e piso × área; ficam as de menor DAP. O mapa destaca o que muda (círculo verde = passa a Corte, estrela vermelha = passa a Rem. 2), há sugestão de UTs vizinhas e exportação em Excel. Com uma UT só, a projeção reproduz exatamente o estado atual. É simulação: não altera os dados.
