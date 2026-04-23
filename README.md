# Gabriel de Rezende Goncalves - Links Hub

Agregador de links estatico, responsivo e bilingue, com troca automatica entre portugues e ingles.

## O projeto

Este repositorio hospeda uma pagina unica de links pessoais, com layout mobile-first, tema escuro e deteccao automatica de idioma.

O foco atual e:

- organizar links principais em uma interface simples e direta;
- manter a pagina extremamente simples de publicar;
- preservar boa performance sem build tool nem framework;
- facilitar iteracoes de conteudo e interface.

## Stack

- HTML5 para estrutura, metadados e logica de idioma
- CSS3 para layout, tema e componentes
- `normalize.css` para reset leve
- `docs/css/custom.css` como unica camada visual da pagina

## Estrutura

- `index.html`: pagina principal, conteudo, SEO, links e traducao PT/EN
- `docs/css/custom.css`: tema, layout, componentes e ajustes responsivos
- `docs/images/icons`: icones SVG efetivamente usados nos links

## Desenvolvimento local

Nao existe processo de build.

```bash
git clone https://github.com/gabireze/links.git
cd links
python -m http.server 8000
```

Depois, abra `http://localhost:8000`.

Tambem funciona abrindo `index.html` diretamente no navegador, mas um servidor local ajuda a validar carregamento de assets e comportamento mais proximo da publicacao real.

## Publicacao

Por ser um site estatico, pode ser publicado em qualquer host simples:

- GitHub Pages
- Netlify
- Vercel
- AWS Amplify
- Firebase Hosting

## Personalizacao

Os ajustes mais comuns ficam nestes pontos:

1. `index.html`
   Atualize bio, links, textos da hero, metatags e dados estruturados.
2. `docs/css/custom.css`
   Ajuste paleta, composicao, hierarquia visual e componentes.
3. `index.html`
   Ajuste os textos do objeto de traducao e os links por idioma.

## Melhorias futuras recomendadas

- versionar localmente avatar, preview social e favicons;
- revisar a necessidade do Google Analytics ou trocar por uma alternativa mais leve;
- adicionar uma pequena rotina de auditoria com Lighthouse ou axe para validar acessibilidade e performance;
- considerar uma estrategia de geolocalizacao por edge/CDN se a selecao automatica de idioma precisar ser baseada em pais real, e nao em idioma/timezone do navegador.

## Licenca

Este projeto continua sob a licenca MIT. Veja [LICENSE.md](LICENSE.md).
