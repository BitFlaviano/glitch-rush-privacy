# Publicar a política de privacidade

A Play Store exige uma **URL pública** para a política. Este diretório já está
pronto para o GitHub Pages.

## Antes de publicar

1. O e-mail de contato já está aplicado: `sousaportoflaviano@hotmail.com`
   (aparece no rodapé da página e no `docs/PRIVACY_POLICY.md`).
2. Se quiser, ajuste a data de "Última atualização".

## Opção A — GitHub Pages (grátis)

```powershell
# dentro da pasta do projeto
git init
git add docs/privacy-site/index.html docs/privacy-site/README.md
git commit -m "Politica de privacidade do Glitch Rush"
git branch -M main
git remote add origin https://github.com/<usuario>/<repo>.git   # crie o repo antes
git push -u origin main
```

No GitHub: **Settings → Pages → Source: Deploy from a branch**,
branch `main`, folder `/docs/privacy-site`. A URL fica
`https://<usuario>.github.io/<repo>/`.

> Observação: o projeto não é um repositório git hoje. Se você não quiser
> versionar o jogo inteiro, crie um repositório só para esta página.

## Opção B — qualquer hospedagem estática

O `index.html` é autossuficiente (CSS embutido, sem imagens nem scripts).
Basta subir em Netlify, Cloudflare Pages, Firebase Hosting, Vercel ou em um
domínio próprio. Qualquer URL `https` serve.

## No Play Console

- **Conteúdo do app → Política de privacidade**: cole a URL final.
- **Dados do app (Data Safety)**: marque que não há coleta nem compartilhamento
  de dados; progresso salvo apenas no aparelho.
- **E-mail de contato**: use o mesmo e-mail publicado na política.
