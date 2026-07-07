# pynkaro-site

Landing page do [Pynkaro](https://pynkaro.com) — assistente de voz com IA para macOS ([código do app](https://github.com/ralbuque/pynkaro)).

Site estático, sem build: `index.html` + `assets/`.

## Publicar (GitHub Pages)

1. Commit e push deste repositório.
2. No GitHub: **Settings → Pages → Source: Deploy from a branch → main / root**.
3. O arquivo `CNAME` já aponta para `pynkaro.com`. No provedor do domínio, configure o DNS:
   - `A` @ → 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - `CNAME` www → `ralbuque.github.io`
4. De volta em **Settings → Pages**, confirme o custom domain `pynkaro.com` e marque **Enforce HTTPS** (o certificado leva alguns minutos).

## Futuro

Dados dos vídeos do dia: o app publicará um `videos.json` neste repositório (ou endpoint), e a página lerá via JavaScript.
