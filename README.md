# Cronograma TR-2036KS

Site estático somente para consulta, baseado na revisão 03 recebida em 07/10/2026. Nomes, percentuais e datas/horários são exibidos como no PDF.

## Arquivos
- index.html: cartões e painel de detalhe por TR.
- styles.css: layout responsivo.
- data.js: percentuais e atividades do cronograma, além dos caminhos opcionais das fotos.
- app.js: renderização somente leitura.
- assets/logo-enesa.png e assets/logo-vale.png: logos.
- assets/fotos/: fotos de campo opcionais.

## Atualizar a revisão
Substitua em data.js os percentuais gerais, resumo de cada TR e as atividades da nova revisão. Preserve as datas como texto com horário, por exemplo 07/10/26 07:30. Para incluir foto, copie o arquivo para assets/fotos/ e cadastre em window.TR_IMAGES, por exemplo: "09": "assets/fotos/tr-09.jpg".

A ordem segue a lista do cronograma. A revisão 03 fornecida não traz coluna de predecessoras; este site não inventa esses vínculos.

## GitHub Pages
Extraia o ZIP diretamente na raiz do repositório: index.html, styles.css, data.js e app.js devem ficar juntos, com assets/ ao lado. Em Settings → Pages escolha Deploy from a branch, branch main, pasta /(root).
