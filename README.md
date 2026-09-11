# Acervo Cleiton Xavier

Protótipo do catálogo pessoal — React + Vite, pronto para publicar no Netlify.

## Rodar localmente (opcional)
Precisa ter o Node.js instalado.

```
npm install
npm run dev
```

Abre em http://localhost:5173

## Publicar

**Opção A — mais simples (Netlify Drop):**
```
npm install
npm run build
```
Isso cria uma pasta `dist/`. Arraste essa pasta em https://app.netlify.com/drop e pronto — link público na hora.

**Opção B — GitHub + Netlify conectados (recomendado a longo prazo):**
1. Crie um repositório no GitHub e suba esta pasta inteira (pode usar "Add file → Upload files" pelo próprio site do GitHub, sem linha de comando).
2. No Netlify, escolha "Import from Git", conecte sua conta GitHub e selecione o repositório.
3. Configuração de build: `npm run build`, pasta de publicação: `dist`.
4. Pronto — toda vez que você atualizar os arquivos no GitHub, o Netlify republica sozinho.

## Estrutura
- `src/App.jsx` — todo o sistema (dados, telas, lógica). É o arquivo que muda quando pedimos ajustes.
- `src/main.jsx` — ponto de entrada, não precisa mexer.
- `index.html` — carrega o Tailwind (estilos) via CDN.
- `public/` — coloque aqui imagens ou ícones que você quiser usar no site (ex.: capas de itens, logo). Um arquivo em `public/capa-batman.jpg` é referenciado no código como `/capa-batman.jpg`.

## Adicionando imagens ou ícones depois
Duas formas:
- Me manda a imagem e o que você quer fazer com ela (ex.: "capa de cada item no Acervo") — eu ajusto `src/App.jsx` e te devolvo os arquivos atualizados, você só sobe de novo no GitHub.
- Ou você mesma solta o arquivo de imagem dentro da pasta `public/` no GitHub e me avisa o nome do arquivo — eu te passo a linha de código exata pra colar, sem precisar mexer no resto.
