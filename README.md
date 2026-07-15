# Portfólio — Pedro Gabriel Castor dos Santos

Site pessoal / portfólio de desenvolvedor Full-Stack, feito em HTML + CSS + JS puros (sem build step, sem dependências de Node).

🔗 Repositório: [PedroDevOps01/Portfolio](https://github.com/PedroDevOps01/Portfolio)

## Estrutura do projeto

```
.
├── index.html              ← página principal do portfólio (entry point do site)
└── curriculos/
    ├── curriculo-v2.html        ← currículo estilizado (linkado no botão "Baixar Currículo")
    ├── curriculo-ats-v2.html    ← versão simples, otimizada para leitura por ATS
    └── curriculo-pedro-gabriel.html  ← versão anterior, mantida como histórico
```

O arquivo `index.html` é o **arquivo principal** do site. Plataformas de deploy estático (GitHub Pages, Netlify, Vercel, Cloudflare Pages) reconhecem `index.html` na raiz do repositório automaticamente como ponto de entrada — não é necessário nenhum arquivo de configuração adicional para publicar.

## Rodando localmente

Não há build nem dependências. Basta abrir o arquivo direto no navegador:

```bash
open index.html
```

Ou servir com qualquer servidor estático simples:

```bash
python3 -m http.server 8000
# depois acesse http://localhost:8000
```

## Deploy em plataforma gratuita

Como o projeto é 100% estático e já usa `index.html` na raiz, o deploy é automático em qualquer uma dessas opções:

- **GitHub Pages**: Settings → Pages → Deploy from branch → `main` / `/ (root)`.
- **Netlify**: "Add new site" → importar o repositório → build command vazio, publish directory `.`.
- **Vercel**: importar o repositório → framework preset "Other" → nenhuma configuração extra necessária.
- **Cloudflare Pages**: conectar o repositório → build command vazio, output directory `.`.

Em todos os casos a plataforma detecta o `index.html` na raiz e publica o site sem passos extras.

## Notas

- O botão "Baixar Currículo" no hero aponta para `curriculos/curriculo-v2.html`.
- As meta tags Open Graph (`og:image`, `twitter:image`) referenciam `og-image.png`, que ainda não existe no repositório — adicione essa imagem na raiz para o preview correto ao compartilhar o link em redes sociais.
