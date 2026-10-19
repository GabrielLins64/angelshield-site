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

## Verificação de propriedade no Google

Publicar no GitHub Pages e cadastrar o endereço no Google Cloud não comprova a propriedade do site para a análise de branding OAuth. A conta usada na verificação precisa ser proprietária ou editora do projeto Google Cloud.

1. No [Google Search Console](https://search.google.com/search-console), adicione uma propriedade do tipo **Prefixo do URL** com `https://gabriellins64.github.io/angelshield-site/`.
2. Escolha **Tag HTML**. A metatag fornecida pelo Search Console fica no `<head>` de `index.html`.
3. Publique o site e confirme que a tag está no HTML da página pública.
4. Clique em **Verificar** no Search Console e confira a confirmação de propriedade. Mantenha a tag no site após a verificação.
5. Para a recusa de branding que pede comprovação de propriedade, aguarde as 24 horas indicadas pelo Google Cloud. Depois, volte a **Branding → Problemas de verificação**, marque **Corrigi os problemas** e solicite uma nova verificação.

A comprovação de propriedade do site e a aprovação de branding são etapas distintas. Se a análise continuar pedindo a propriedade do domínio completo, verifique o domínio exigido ou use um domínio próprio que consiga comprovar. [Orientações para página inicial OAuth](https://support.google.com/cloud/answer/13807376) e [métodos de verificação do Search Console](https://support.google.com/webmasters/answer/9008080?hl=pt-BR).

## Prévia local

Na raiz do repositório, execute `python3 -m http.server 8766 --bind 127.0.0.1` e abra `http://127.0.0.1:8766/`. Confira também `/privacidade/`. Não há dependências, JavaScript, fontes externas, anúncios ou ferramentas de análise de visitas.
