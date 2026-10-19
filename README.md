# Site do AngelShield

Página pública do AngelShield, com apresentação dos recursos, informações sobre o backup opcional no Google Drive, suporte e política de privacidade.

- Página inicial: https://gabriellins64.github.io/angelshield-site/
- Política de privacidade: https://gabriellins64.github.io/angelshield-site/privacidade/
- Suporte: https://github.com/GabrielLins64/angelshield-site/issues

## Publicação

O GitHub Pages publica a raiz da branch `main`. O arquivo `.nojekyll` indica que o conteúdo é HTML estático, sem etapa de build própria. A publicação usa o repositório `GabrielLins64/angelshield-site`.

## Estrutura

- `index.html`: apresentação do AngelShield, recursos, backup no Drive e links de suporte e privacidade.
- `privacidade/index.html`: texto da política de privacidade.
- `assets/site.css`: estilos compartilhados e layout para desktop e celular.
- `assets/angelshield.png`: ícone original da extensão.
- `assets/cofre.png`: captura da interface com dados fictícios, reaproveitada das imagens da Chrome Web Store.

Para atualizar a política, edite `privacidade/index.html` e revise a data da atualização se o conteúdo mudar. A versão de referência também fica em `docs/privacy.html` no projeto AngelShield; mantenha o texto dos dois arquivos alinhado.

Ao publicar esta refatoração, atualize a URL da política na Chrome Web Store para o caminho `/privacidade/`. No Branding do Google Cloud, use a raiz do site como página inicial e o caminho `/privacidade/` como política. A política continua acessível por um link na página inicial.

## Prévia local

Na raiz do repositório, execute `python3 -m http.server 8766 --bind 127.0.0.1` e abra `http://127.0.0.1:8766/`. Confira também `/privacidade/`. Não há dependências, JavaScript, fontes externas, anúncios ou ferramentas de análise de visitas.
