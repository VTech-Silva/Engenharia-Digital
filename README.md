# Engenharia em Dados — Painel de marcos

Site estático e somente para consulta, preparado para GitHub Pages e para o domínio `engenhariaemdados.com.br`.

## Estrutura
- `index.html`: painel de marcos e janelas de detalhe.
- `styles.css`: layout responsivo.
- `app.js`: exibição e navegação entre marcos, TRs e atividades.
- `data.js`: dados da revisão 03, cartões dos marcos e caminhos das imagens.
- `assets/logo-enesa.png` e `assets/logo-vale.png`: logos.
- `assets/fotos/`: imagens opcionais de cada marco/TR.
- `CNAME`: domínio personalizado do GitHub Pages.

## Atualizar dados e adicionar marcos
Edite `data.js`. As datas e os nomes das atividades da revisão 03 estão cadastrados como texto e são exibidos sem alteração. Para inserir fotos, coloque o arquivo em `assets/fotos/` e informe o caminho em `window.TR_IMAGES` (chave com o número da TR, por exemplo `"09": "assets/fotos/tr-09.jpg"`). Para fotos dos cartões de marcos, use `window.MILESTONE_IMAGES` com chaves `silos`, `tr2020-11` ou `tr2020-12`.

Os quatro cartões tracejados aparecem como espaços para novos marcos. A lista é controlada no início de `app.js`, no array `milestones`; duplique um item de marco para criar outro cartão. Para habilitar dados de um novo marco, configure sua ficha no mesmo arquivo seguindo o modelo dos marcos existentes.

Silos e TR-2020KS-11/12 estão preparados como fichas, mas sem datas, percentuais ou atividades porque esses dados ainda não foram fornecidos. Não há campos de edição no site.

## Publicar no GitHub Pages
Extraia o conteúdo do ZIP na raiz do repositório (o `index.html` precisa ficar na raiz). Em **Settings → Pages**, publique a branch principal pela pasta raiz. O arquivo `CNAME` já declara `engenhariaemdados.com.br`; configure os registros DNS no provedor onde o domínio foi comprado, seguindo as instruções atuais do GitHub Pages para domínio personalizado. Ative HTTPS quando a configuração do domínio for validada.
