# Saint Nicholas House B — Tour 360° | Publicação no GitHub Pages

Este pacote contém o tour 360° pronto para publicar. Siga os passos abaixo.

## Estrutura dos arquivos
```
index.html          → a página do tour (com as meta tags de preview)
preview.jpg         → imagem que aparece no WhatsApp/redes (1200×630)
images/
  entrada.jpg       → cena 01
  hall.jpg          → cena 02
  escada.jpg        → cena 03
  corredor.jpg      → cena 04
  cozinha1.jpg      → cena 05
  cozinha2.jpg      → cena 06
  logo.png          → logo Leevin Student
  map.png           → ícone Google Maps
```

## Passo 1 — Criar o repositório
1. Entre em https://github.com e faça login (ou crie a conta).
2. Clique em **New repository**.
3. Dê um nome — por exemplo: `tour-saint-nicholas`. Anote esse nome.
4. Deixe **Public** (o GitHub Pages gratuito exige público).
5. Crie o repositório.

## Passo 2 — Subir os arquivos
1. No repositório, clique em **Add file → Upload files**.
2. Arraste TODO o conteúdo deste pacote (o `index.html`, o `preview.jpg` e a pasta `images`).
   - Importante: mantenha a pasta `images` com esse nome.
3. Clique em **Commit changes**.

## Passo 3 — Ativar o GitHub Pages
1. No repositório, vá em **Settings → Pages**.
2. Em **Source**, escolha **Deploy from a branch**.
3. Branch: **main** / pasta: **/(root)**. Salve.
4. Aguarde 1–2 minutos. O GitHub mostrará a URL, algo como:
   `https://SEU-USUARIO.github.io/tour-saint-nicholas/`

## Passo 4 — Corrigir a URL nas meta tags (ESSENCIAL para o preview)
1. Abra o `index.html` no GitHub (clique nele → ícone de lápis para editar).
2. Logo no topo há um bloco com 4 linhas contendo `SEU-USUARIO.github.io/NOME-DO-REPO`.
3. Troque as 4 ocorrências pela sua URL real. Exemplo:
   - de: `https://SEU-USUARIO.github.io/NOME-DO-REPO/preview.jpg`
   - para: `https://joaosilva.github.io/tour-saint-nicholas/preview.jpg`
4. Commit.

## Passo 5 — Testar o preview ANTES de mandar no WhatsApp
O WhatsApp guarda o preview em cache; se testar errado, o preview quebrado gruda.
1. Abra https://developers.facebook.com/tools/debug/
2. Cole a URL do tour e clique em **Debug**.
3. Se aparecer a imagem e o título corretos, está pronto.
4. Se mudar algo depois, use **Scrape Again** nessa mesma ferramenta para atualizar o cache.

## Observações
- **É público**: qualquer pessoa com o link acessa. Para mostrar só a gerentes/equipe
  isso costuma bastar (link não divulgado), mas não é privacidade garantida.
- **Endereço**: no `index.html`, procure por `- Cork, Ireland` para adicionar a rua completa se quiser.
- **Ajuste das setas**: se alguma seta de navegação apontar para o lado errado,
  edite os valores `yaw`/`pitch` no bloco `scenesData` dentro do `index.html`.
