
# Projeto com 3 projetos de HTML e CSS
### Projeto com 4 páginas/telas incluindo uma página principal que se redireciona para 3 projetos simples de HTML e CSS. Página de QR-CODE, Cartão de Preview de postagem e Cartão de Serviços/Venda

[<img src="./images/readme/main.gif">](https://benssssss.github.io/7-css-html-projects/)

[<img src="./images/readme/stat-back.gif">](https://github.com/benssssss/7-css-html-projects)

---

# Processo

## Design
### Design, layout e criação de assets feito usando Pacote Adobe junto ao layout obtido no Frontend Mentor

1 - Obter referência e layout

## Planejamento

1 - Fazer desenho de caixas (grid-flex) antes de escrever qualquer código, definindo quais elementos serão usados (desenho no pdf abaixo)

### Links para assets, design, planejamento e referência de layout


[Página QR Code](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H)

[Cartão de Preview de postagem](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS)

[Cartão de Serviços/Venda](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62)

---

## Código

### OBS: Comecei escrevendo o código de cada página por vez, como não são de tamanha complexidade eu resolvi junta-las em um único projeto e fiz uma pagina principal para facil acesso das outras páginas

---

### 1 - Página principal
#### Comecei escrevendo esse código por ultimo,  

a - Fiz um botão de volta em todas as páginas para que seja possivel voltar para a página principal e entrar em outra página, usei um .css separado (.elemento-voltar.css) para criar um container e usar seu estilo em todas as outras paginas, o HTML foi inserido sobre as "main's" em um "header"

b - Usei fotos dos cartões na página principal, depois de alinhar fiz um :hover com a cor primaria do respectivo cartão em um "background-color:;" e "opacity:;" para ser possível ver o cartão quando o hover ativo, tambem coloquei um texto para indicar a area clicavel com o link para determinada página

c - Fiz um responsivo simples em (1080px) alterando o "Flex-direction" para "flex-direction: column;" no qual estava no padrão "flex-direction: row;", nessa mudança a minha página quebrou, o main não estava ocupando 100% da tela, e estava cortando a seção do qr-code, isso porque meu main estava com largura "height: 100vh;" eu consegui arrumar em pouco tempo, apenas alterando de "height" para "min-height: 100vh;"  

---

### 2 - Página QR Code 

a - Criei um main, inseri a imagem (qr-code), fiz uma div para separar os textos (h1 e p), 

[Fonte que usei para ajuste do tamanho]("https://www.browserstack.com/guide/how-to-resize-image-using-css")

b - Usei display: flex; para centralzar o cartão horizontalmente (justify-content) e verticalmente (align-items)

*Para o botão de voltar, adicionei o codigo (HTML) no header e linkei o (.elemento-voltar.css) no html da página 

- Usei uma propriedade que nunca havia usado antes "Object-fit:;" que serve como um background-size para "img", precisei dela pra resolver o problema de ajustar o tamanho da imagem ao tamanho do cartão

```
.card-image {
    object-fit: cover;
}
```

- Não tem responsivo por ter tamanho fixo (320px), assim se adaptando as menores telas (telas mobile pequenas)  

---

### 3 - Cartão de Preview de postagem

a - Criei um container geral do cartão, depois separei ele em 4 partes

b - Imagem "picture/img" (defini um tamanho)

c - Titulo, descrição e data de publicação 

troquei as fontes e tamanhos - Nesses acima usei space-between para fazer o posicionamento dos elementos em cada extremo (topo e fundo)

d - Criador do conteudo (adicionei o img), e coloquei display: flex; no container, posicionando a foto e texto um do lado do outro

*Para o botão de voltar, adicionei o codigo (HTML) no header e linkei o (.elemento-voltar.css) no html da página 

---

### 4 - Cartão de Serviços/Venda

Como esse projeto tem responsividade (960px e 1200px), comecei com mobile first
Uma nova propriedade 

- Uma nova propriedade foi utilizada para responsividade das fotos, assim mostrando a foto mobile (com tamanho menor) abaixo de 960px e mostrando a foto original (desktop) acima dessa resolução

```
<picture>
    <source media="(min-width: 960px)" srcset="./image-header-desktop.jpg"/>
    <img src="./image-header-mobile.jpg">
</picture>
```

### 5 - .elemento-voltar.css 

a - Usei display: block para poder mover os elementos, 

b - top: 0, left: 0 e depois um padding de 15px em todos os lados 

### Fazer versionamento quando;
- Houveram versionametos nos projetos individuais (que foram removidos), um novo projeto foi criado e um novo versionamento aconteceu apenas quando a página principal já estava em estagio avançado

- Html escrito
- Css escrito
- Clean code
- Ajuste de metadata e inserção de "Readme.md"

# Tecnologias utilizadas
- HTML5 Markup 
- CSS
- Clean Code
- Photoshop
- Illustrator
- Responsividade

# O que eu aprendi

### CSS
a - Fazer um .css individual para uma parte especifica da página (containezar), como o que eu usei no botão de "voltar"

b - Propriedade para alterar tamanho de imagens
```
.card-image {
    object-fit: cover;
}
```

### HTML

```
<picture>
    <source media="(min-width: )" srcset="/>
    <img src="">
</picture>
```

# Dificuldades

### "Cartão de Serviços/Venda"

1 - Responsividade do projeto , na hora de alterar as imagens com o mudar da resolução, resolvida usando o conjunto "picture + source e srcset"

2 - Fazer a sobreposição da "cor roxa" sobre a imagem, resolvida usando "position: absolute; e "position: relative; e mudança de opacidade" 

---

# Autor
### Jefferson Augusto (a.k.a Benssssss) 
## [LinkedIn](https://www.linkedin.com/in/benssssss/)

## Projeto n.º7
