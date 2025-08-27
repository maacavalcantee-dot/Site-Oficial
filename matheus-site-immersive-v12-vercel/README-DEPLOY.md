
# Deploy na Vercel — cantormatheuscavalcante.com.br

## Passo a passo (upload do ZIP)
1. Entre em https://vercel.com/new
2. Clique em **"Upload"** e envie este pacote `v12-vercel`.
3. Em **Project Settings**:
   - Framework preset: **Other / None**
   - Build Command: **(vazio)**
   - Output Directory: **/** (raiz) — é um site estático puro
4. Clique em **Deploy**.

## Ligar o domínio
1. No projeto: **Settings → Domains → Add** → `cantormatheuscavalcante.com.br`
2. No painel do seu registrador (onde comprou o domínio), crie/ajuste os DNS:
   - **A (apex @)** → `76.76.21.21`
   - **CNAME (www)** → `cname.vercel-dns.com.` (com ponto final, se o painel pedir)
3. Volte na Vercel e marque **cantormatheuscavalcante.com.br** como **Primary**.
4. (Opcional) Ative a opção **redirect www → apex** nas configurações do domínio.

## Checagens após publicar
- **Meta Pixel** (ID: 319335981257451): use a extensão **Meta Pixel Helper** → deve mostrar **PageView** ao abrir e **Lead** ao enviar o formulário.
- **GA4** (ID: G-2S3YLJF43Q): abra o **Realtime**/**DebugView** no Google Analytics e verifique os acessos/eventos.
- **Sitemap/robots**: 
  - https://cantormatheuscavalcante.com.br/robots.txt
  - https://cantormatheuscavalcante.com.br/sitemap.xml
- **Open Graph**: compartilhe o domínio no Whats/FB e veja o cartão de preview.

## Dúvidas comuns
- *“Não aparece o PageView do Pixel”*: com o site local (file://) não carrega. Precisa estar publicado em HTTPS.
- *“GA não mostra nada”*: use o **DebugView** do GA e aguarde alguns minutos; se necessário, teste em aba anônima.

Qualquer ajuste, me chame aqui que eu atualizo o projeto.
