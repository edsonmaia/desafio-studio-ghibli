# Projeto Studio Ghibli - Desafio 5 CodeLab - Responsividade

## Efeitos :hover nos links e botões

~~~css
.link {
    /* ... */
    transition: all ease .5s;
}

.botao {
    /* ... */
    transition: all ease .5s;
}

/* efeito hover */
.link:hover {
    background-color: #F1A5B1;
}

.botao-primario:hover, .botao-secundario:hover {
    background-color: #f8f8f8;
    color: #0B0A0A;
    border-color: transparent;
}

~~~

## Ajuste no HTML

1. Dentro da tag header temos um link a que acomoda a logo da nossa aplicação. Defina a class "logo" para a img que está dentro da tag a.

~~~html
    <img class="logo" src="images/logo.svg" alt="Logo do Studio Ghibli" />
~~~

2. Dentro da tag h2 do título "A VIAGEM DE CHIHIRO", apague a tag '<br>' de quebra de linha. Vamos controlar essa quebra pela propriedade 'width' do '.titulo'.

3. Salve as alterações.

## Responsividade

~~~css
.ilustracao {
    width: 100%;
    height: 100%;
    background-image: url('../images/image.svg');
    background-repeat: no-repeat;
    /* border: 1px solid red; */
    background-position: center;
    background-size: cover;
}

~~~

~~~css
/* responsividade */
/* Telas grandes (desktops) */
@media (max-width: 1200px) {
    body {
        width: 100%;
        height: 100%;
        padding-inline: 5%;
        margin-bottom: 20px;
    }
    .conteudo {
        flex-direction: column;
    }
    .ilustracao {
        order: 1;
        height: 424px;
        background-size: contain;
    }
    .descricao {
        order: 2;
    }
}

/* Telas medias (tablets) */
@media (max-width: 768px) {
    .header {
        width: 100%;
        height: 128px;
    }
    .header .logo {
        height: 64px;
    }
    .conteudo {
        width: 100%;
    }
    .ilustracao {
        height: 240px;
        background-size: contain; /* opcional */
    }
    .descricao .titulo-chapeu {
        font-size: 16px;
        line-height: 22px;
        font-weight: 700;
    }
    .descricao .titulo {
        font-size: 40px;
        line-height: 44px;
        font-weight: 800;
        width: 270px;
    }
    .descricao p {
        font-size: 16px;
        line-height: 24px;
        font-weight: 500;
    }
    .botoes {
        flex-direction: column;
        height: 100%;
    }
    .botao {
        width: 100%;
    }
}

/* Telas menores 600, 575, 500 */
@media (max-width: 500px) {
    .header {
        justify-content: center;
    }
    .header .nav-links {
        display: none;
    }
}

/* Telas pequenas (mobile) */
@media (max-width: 390px){
    .header {
        height: 96px;
    }
    .header .logo {
        height: 48px;
    }
    .ilustracao {
        height: 184px;
    }
}

~~~

Salve as alterações e teste no navegador.

## Desafio proposto

Eu deixo como desafio o desenvolvimento de mais funcionalidades para a nossa aplicação. Por exemplo:

1ª sugestão criar o link no botão primário para acessar o vídeo do filme disponível na Netflix
[Link na Netflix](https://www.netflix.com/title/60023642)

2ª sugestão criar o link no botão secundário para acessar o trailer disponível no Youtube
[Link no YouTube](https://www.youtube.com/watch?v=SgZI655GgHk)

[Link da página oficial sobre o Filme A Viagem de Chihiro](https://studioghibli.com.br/filmografia/a-viagem-de-chihiro/)

## Considerações

Nesta aula vimos como implementar o efeito hover nos links e botões, e por fim como finalizar o projeto completo do Desafio 5 do Studio Ghibli com base no Figma do Projeto, aplicando os recursos de responsividade na nossa aplicação.
Na próxima aula extra vamos fazer a publicação deste projeto no GitHub e no GitHub Pages.

Salve Devs, até as próximas!
