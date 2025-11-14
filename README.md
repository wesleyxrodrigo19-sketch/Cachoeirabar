# Cachoeira Bar e Petiscaria — site pronto para hospedar

Este repositório contém a versão estática do sistema que você enviou, preparada para publicar online (GitHub Pages, Netlify, Vercel ou similar).

Arquivos incluídos:
- `index.html`         — dashboard / área administrativa (renomeado a partir de "CACHOEIRA BAR.html")
- `tela-espera.html`  — tela de espera que abre em outra janela
- `logo-cachoeira.svg` — logotipo simples (substitua pelo PNG/JPG que você enviou, se desejar)

Como publicar online (opções rápidas):

1) Publicar com GitHub Pages (passos rápidos)
- Crie um novo repositório no GitHub (por exemplo `cachoeira-bar`).
- No seu computador:
  - git init
  - git add .
  - git commit -m "Site Cachoeira Bar"
  - git branch -M main
  - git remote add origin https://github.com/SEU_USUARIO/SEU_REPO.git
  - git push -u origin main
- No GitHub: vá em Settings → Pages → Source → selecione "main" branch e root (/) → Save.
- A URL ficará disponível em alguns minutos: `https://SEU_USUARIO.github.io/SEU_REPO/`

2) Netlify (arrastar e soltar)
- Acesse https://app.netlify.com/drop e arraste a pasta com os arquivos (index.html deve estar na raiz).
- Netlify cria um site público automaticamente.

3) Vercel
- Faça login no Vercel e crie um novo projeto apontando para o repositório. É um deploy automático para sites estáticos.

Importante / dicas
- Substituir o logotipo:
  - Se você tiver a imagem que enviou (PNG), renomeie-a para `logo-cachoeira.png` e envie para a raiz do site. Se preferir manter o SVG, os arquivos já referenciam `logo-cachoeira.svg`.
  - Se quiser usar o PNG, abra `index.html` e `tela-espera.html` e troque `logo-cachoeira.svg` por `logo-cachoeira.png` (ou mantenha ambos).
- Dados persistem no navegador via `localStorage`. Ao publicar, o site continuará a armazenar dados no browser do usuário que usar a aplicação.
- Para produção com múltiplos usuários/environments, recomendo conectar um backend (Firebase/Firestore, Supabase ou API própria) para armazenar pedidos e sincronizar a tela de espera em tempo real.

O que eu já fiz:
- Converti o seu HTML principal para `index.html` (padrão para hospedagem estática) e ajustei referências para um logotipo SVG incluído.
- Mantive a `tela-espera.html` como estava, ajustando também para usar o SVG.
- Adicionei um logotipo em SVG leve para permitir deploy imediato sem upload de imagem.

Próximos passos que posso ajudar a executar:
- Subir esses arquivos diretamente para um repositório GitHub (posso fornecer comandos passo a passo ou um script).
- Gerar um pequeno workflow (GitHub Actions) que publique automaticamente no GitHub Pages ao push.
- Substituir o SVG pelo PNG que você enviou (posso gerar o base64 se quiser incorporar a imagem diretamente).
- Integrar com Firebase/Realtime para sincronização entre painéis (tela principal e tela de espera) em tempo real.

Diga qual opção prefere (ex.: "publique no meu GitHub" ou "gere workflow para GitHub Pages" ou "substituir logo pelo PNG"), e eu preparo os comandos/arquivos.
```