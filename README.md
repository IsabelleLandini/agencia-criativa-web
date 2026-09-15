# 🚀 Agência Criativa Web

Projeto de landing page desenvolvido com **HTML5, SASS (SCSS), CSS3 e Node.js**, com foco em prática de layout moderno, responsividade, organização de código, boas práticas de desenvolvimento front-end.

---

## Sobre o projeto

A **Agência Criativa Web** é uma landing page fictícia criada para simular o site de uma agência digital.

Nesta versão do projeto foi realizada uma refatoração completa dos estilos utilizando **SASS (SCSS)**, com o objetivo de tornar o código mais organizado, reutilizável, modular e escalável.

### Principais melhorias implementadas:

* Aplicação da metodologia **BEM (Block, Element, Modifier)**
* Organização dos estilos em arquivos parciais (Partials)
* Utilização de variáveis SASS para cores, fontes e espaçamentos
* Criação de mixins reutilizáveis
* Uso de aninhamento de seletores
* Utilização de operadores SASS
* Separação entre layout, componentes e estilos globais
* Redução da duplicação de código
* Melhor manutenção e escalabilidade do código
* Preservação da responsividade em diferentes dispositivos

---

## Layout do projeto

O site é composto por:

*  **Home** – apresentação principal com banner e chamada para ação
* **Sobre Nós** – descrição da agência e valores
* **Serviços** – cards com os principais serviços oferecidos
* **Depoimentos** – feedback de clientes fictícios
*  **Contato** – formulário e informações de contato

---

## Tecnologias e conceitos utilizados

### Tecnologias 

* HTML5
* CSS3
* SASS (SCSS)
* Node.js

### Conceitos aplicados

* Metodologia BEM
* Flexbox
* CSS Grid
* Media Queries
* Variáveis SASS
* Mixins
* Partials
* Aninhamento de seletores
* Operadores SASS
* Componentização de estilos
* Responsividade

---

## Responsividade

O projeto é totalmente responsivo e se adapta a:

* 💻 Desktop
* 📱 Tablets
* 📱 Celulares

---

## 📂 Estrutura do projeto

```text
📁 agencia-criativa-web/
│ 
├── css/
│     ├── estilos.css 
│     ├── estilos.css.map 
│     └── estilos.min.css
│ 
├── scss/ 
│     ├── _variaveis.scss 
│     ├── _mixins.scss 
│     ├── _base.scss 
│     ├── _layout.scss 
│     ├── _componentes.scss 
│     └── estilos.scss 
│
├── imagens/
│     ├── banner-grande.jpg
│     ├── banner-media.jpg
│     ├── banner-pequena.jpg
│     ├── banner-grande.webp 
│     ├── banner-media.webp 
│     └── banner-pequena.webp
│
├── relatorios/
│     ├── lighthouse-antes.pdf
│     ├── lighthouse-antes.png
│     ├── lighthouse-depois.pdf
│     └── lighthouse-depois.png
|
├── index.html
├── index_original.html
├── package.json
├── package-lock.json
├── screenshot.png
└── README.md
```

---

## Como executar o projeto

1. Baixe ou clone o repositório:

```bash
git clone https://github.com/IsabelleLandini/agencia-criativa-web.git 
```

2. Acesse a pasta do projeto

```bash
cd agencia-criativa-web
```

3. Instale as dependências

```bash
npm install
```

4. Compile o SASS

```bash
npx sass --watch scss/estilos.scss css/estilos.css
```

5. Execute o projeto

Abra o arquivo `index.html` no navegador ou utilize a extensão Live Server do VS Code.

---

## Refatoração com SASS

Durante esta etapa do projeto foram aplicados os principais recursos do SASS:

* Estrutura modular utilizando Partials
* Importação moderna com `@use`
* Variáveis para cores, fontes e espaçamentos
* Mixins reutilizáveis para componentes
* Aninhamento de seletores
* Operadores para cálculos de espaçamento
* Organização dos estilos em arquivos específicos

---

## Otimização de Performance

Nesta etapa, o projeto passou por uma análise de performance utilizando o **Lighthouse**, seguida da aplicação de otimizações para melhorar o carregamento e a qualidade geral da página.

### Problemas identificados

Na análise inicial foram identificados principalmente:

* CSS bloqueando a renderização inicial
* Imagens com oportunidade de melhoria na entrega e no tamanho dos arquivos
* Imagens sem dimensões explícitas
* Ausência de descrição para SEO
* Código HTML e CSS sem minificação

### Otimizações realizadas

* Conversão das imagens para **WebP**
* Utilização de `srcset`, `sizes` e `<picture>` para fornecer imagens adequadas a diferentes tamanhos de tela
* Definição de `width` e `height` nas imagens
* Ajuste do CSS para preservar a proporção das imagens
* Não aplicação de `loading="lazy"` na imagem principal, pois ela participa do carregamento inicial e do LCP; nesse caso o carregamento tardio poderia prejudicar a performance
* Minificação dos arquivos HTML e CSS
* Remoção de código CSS duplicado
* Adição de meta description para melhorar o SEO
* Análise do código JavaScript, que não possui código próprio no projeto e, portanto, não exigiu otimização
* Manutenção da responsividade após as otimizações

### Resultados do Lighthouse

| Categoria | Antes | Depois |
| --------- | ----: | -----: |
| Performance | 100 | 100 |
| Accessibility | 100 | 100 |
| Best Practices | 100 | 100 |
| SEO | 91 | 100 |

A pontuação de **SEO aumentou de 91 para 100**, enquanto as demais categorias mantiveram a pontuação máxima.

### Métricas de carregamento

| Métrica | Antes | Depois |
| ------- | ----: | -----: |
| FCP | 1,1 s | 1,1 s |
| LCP | 1,4 s | 1,3 s |
| TBT | 0 ms | 0 ms |
| CLS | 0 | 0 |
| Speed Index | 1,1 s | 1,1 s |

O **LCP apresentou uma melhora de 0,1 s**, passando de 1,4 s para 1,3 s após as otimizações.

### Comparativo dos resultados

#### Antes

![Resultados do Lighthouse antes das otimizações](./relatorios/lighthouse-antes.png)

#### Depois

![Resultados do Lighthouse depois das otimizações](./relatorios/lighthouse-depois.png)

---

## 📸 Preview do projeto

<p align="center">
  <strong>Landing Page da Agência Criativa Web</strong><br><br>
  <img src="./screenshot.png" width="900px" alt="Preview do projeto">
</p>

---

## 👩🏻‍💻 Autora

Desenvolvido por **Isabelle Landini**. 

✨ Projeto para estudo e portfólio pessoal em desenvolvimento web.
