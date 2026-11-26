# carlosmenezes.des.br

Portfólio de Carlos Menezes, Product Designer. Site estático, publicado pelo GitHub Pages.

## Estrutura

```
index.html                 o site inteiro (home, currículo e cases, por rotas #/home, #/curriculo, #/veloe, #/digio, #/tesouro)
assets/img/                imagens dos cases, logos e fotos
assets/fonts/              Archivo e Anton, hospedadas no próprio site
assets/Carlos-Menezes-Curriculo-Product-Designer.pdf
favicon.svg, favicon.png, apple-touch-icon.png
og-image.png               imagem que aparece ao compartilhar o link
CNAME                      domínio próprio (carlosmenezes.des.br)
.nojekyll                  publica os arquivos como estão
404.html                   leva qualquer endereço inexistente para a home
robots.txt, sitemap.xml
```

## Publicar no GitHub Pages

1. Crie um repositório público no GitHub, por exemplo `portfolio`.
2. Envie todo o conteúdo desta pasta para a raiz do repositório, incluindo `CNAME` e `.nojekyll`
   (arquivos que começam com ponto podem ficar ocultos no Finder: no Mac, Cmd + Shift + . mostra os ocultos).
3. No repositório: **Settings → Pages → Build and deployment**.
   Em *Source*, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`, e salve.
4. Ainda em **Settings → Pages**, em *Custom domain*, confirme `carlosmenezes.des.br` e salve.

## Apontar o domínio (no Registro.br ou onde o DNS estiver)

Crie estes registros:

| Tipo  | Nome | Valor                   |
|-------|------|-------------------------|
| A     | @    | 185.199.108.153         |
| A     | @    | 185.199.109.153         |
| A     | @    | 185.199.110.153         |
| A     | @    | 185.199.111.153         |
| AAAA  | @    | 2606:50c0:8000::153     |
| AAAA  | @    | 2606:50c0:8001::153     |
| AAAA  | @    | 2606:50c0:8002::153     |
| AAAA  | @    | 2606:50c0:8003::153     |
| CNAME | www  | CarlosMenezes91.github.io   |

A propagação pode levar algumas horas.
Quando o GitHub confirmar o domínio, marque **Enforce HTTPS** em Settings → Pages.

Recomendado: verifique o domínio em **Settings (da sua conta) → Pages → Add a domain**,
para impedir que outra conta use o seu domínio.

Referência: https://docs.github.com/pt/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site

## Atualizar o site

Substitua os arquivos alterados no repositório e faça o commit. O GitHub Pages publica em seguida.
