# CLAUDE.md — BOLSAJUVENTUDERURAL

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** BOLSAJUVENTUDERURAL
**Nicho:** Educação
**Keywords:** O site bolsa juventude rural tem o foco de levar educacao para
**Paleta de cores:** gold | **Fonte:** inter

O site bolsa juventude rural tem o foco de levar educação para crianças e jovens das mais diversas áreas rurais do nosso Brasil, de forma simples e gratuita. A nossa criação faz parte parte do movimento de dialogar com a sociedade mais carentee, ao mesmo tempo, participar da disputa pelos sentidos da educação no espaço rural. Convidamos a todos que defendem um ensino gratuito de qualidade a nos acompanharem. Oferecemos conteúdo gratuito e de qualidade, atividades pedagógicas durante a quarente, para que as crianças e jovens não se afastem do ambiente escolar e continuem se preparando para o futuro! Todo o nosso conteúdo pode ser acesso através do nosso site e de forma 100% gratuita.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-I |
| Hero | Hero-A |
| Features | Features-J |
| About Section | About-I |
| Posts | Posts-A |
| Footer | Footer-H |
| Página Sobre | Sobre-A |
| Página Contato | Contato-A |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
