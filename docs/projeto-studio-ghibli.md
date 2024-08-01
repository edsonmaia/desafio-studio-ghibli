# Projeto Studio Ghibli - Desafio 5 CodeLab

## Projeto FIGMA

[Desafio 5 - Studio Ghibli](https://www.figma.com/design/Yb9IBH56g7T1hdIyZ3BMNO/Desafios---CodeLab?t=txmBd1xzhCpgPS0O-0)

## Repositório do Desafio no GitHub

[Repositório dos Desafios no GitHub](https://github.com/iuricode/desafios-frontend)

> Com base nas instruções do desafio e do arquivo Figma feito pelo Iuri Silva do CodeLab, vamos criar o seguinte projeto

## Criar o projeto web

1. Dentro de uma unidade C: ou D: crie a pasta `desafio-5-studio-ghibli`
2. Clique na pasta jordan-shoes com o botão direito e escolha `Abrir com Code`
3. Dentro da pasta raiz do projeto crie as pastas `css` e `images`


## Copiar as images para a pasta images

1. Baixe o arquivo zip com as imagens

[ZIP das imagens](https://drive.google.com/file/d/1HcOpp15YIjrjS8rxDOhmpaRWZao0zzZf/view?usp=sharing)

2. Extrai os arquivos do zip
3. Copie e cole eles para dentro da pasta `images` do seu projeto

## Arquivo index.html

1. Na raiz do projeto crie o arquivo `index.html`
2. Faça os seguinte código:

~~~html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8" />
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Andada+Pro:ital,wght@0,400..840;1,400..840&family=Archivo:ital,wght@0,100..900;1,100..900&display=swap" rel="stylesheet">
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="icon" href="images/favicon.png" />
    <title>Studio Ghibli</title>
    <link rel="stylesheet" href="css/style.css" />
</head>
<body>
<header class="header">
        <a href="#">
            <img src="images/logo.svg" alt="Logo do Studio Ghibli" />
        </a>
        <nav class="nav-links">
            <a href="" class="link">
                <img src="images/icones/logo-google.svg" alt="Ícone do google" />
            </a>
            <a href="" class="link">
                <img src="images/icones/logo-facebook.svg" alt="Ícone do facebook" />
            </a>
            <a href="" class="link">
                <img src="images/icones/logo-twitter.svg" alt="Ícone do twitter" />
            </a>
            <a href="" class="link">
                <img src="images/icones/logo-instagram.svg" alt="Ícone do instagram" />
            </a>
        </nav>
    </header>

    <main>
        <section class="conteudo">

            <div class="descricao">
                <h3 class="titulo-chapeu">HAYAO MIYAZAKI</h3>
                <h2 class="titulo">A VIAGEM <br>DE CHIHIRO</h2>
                <p>Chihiro chega a um mundo mágico dominado por uma bruxa. Aqueles que a desobedecem são transformados em animais.</p>
            
                <div class="botoes">
                    <button class="botao botao-primario">
                        <svg id="icon-play" width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M21.9834 10.4127L8.47594 2.15051C8.19267 1.97782 7.86865 1.88338 7.53696 1.87683C7.20526 1.87028 6.87777 1.95186 6.58791 2.11323C6.29804 2.27461 6.05618 2.51 5.88702 2.79539C5.71785 3.08078 5.62744 3.40594 5.625 3.73769V20.2621C5.62744 20.5938 5.71785 20.919 5.88702 21.2044C6.05618 21.4898 6.29804 21.7252 6.58791 21.8865C6.87777 22.0479 7.20526 22.1295 7.53696 22.1229C7.86865 22.1164 8.19267 22.0219 8.47594 21.8493L21.9834 13.5871C22.2558 13.4213 22.4809 13.1882 22.6371 12.9102C22.7934 12.6322 22.8754 12.3187 22.8754 11.9999C22.8754 11.681 22.7934 11.3675 22.6371 11.0896C22.4809 10.8116 22.2558 10.5785 21.9834 10.4127ZM7.875 19.5796V4.42019L20.265 11.9999L7.875 19.5796Z" fill="#0B0A0A"/>
                        </svg>
                        ASSISTIR AGORA
                    </button>
                    <button class="botao botao-secundario">
                        ASSISTA O TRAILER
                    </button>
                </div>
            </div>

            <div class="ilustracao"></div>

        </section>
    </main>
    
</body>
</html>

~~~

> Dentro da tag head já estão os links do Google Fonts, do Favicon e da página de Estilos.

3. Salve as alterações.

## Arquivo CSS

1. Dentro da pasta `css` crie o arquivo `style.css`
2. Faça o seguinte código:

~~~css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    width: 100%;
    height: 100vh;
    background-image: url('../images/wallpaper.png');
    background-size: cover;
    color: #fff;

    display: flex;
    flex-direction: column;
    align-items: center;

}

h1, h2, h3, h4, h5, h6 {
    font-family: 'Andada Pro', serif;
}

p, button {
    font-family: 'Archivo', sans-serif;
}

.header {
    width: 80%;
    height: 176px;

    display: flex;
    align-items: center;
    justify-content: space-between;
}

.header .nav-links {
    display: flex;
    gap: 24px;
}

.nav-links .link {
    width: 40px;   
    height: 40px;
    border-radius: 50%;
    background-color: #f8f8f850;
    border: 1px solid #fff;

    display: flex;
    align-items: center;
    justify-content: center;
}

main {
    width: 80%;
    height: 100%;

    display: flex;
    align-items: center;
    justify-content: center;
}

.conteudo {
    width: 100%;
    height: 100%;

    display: flex;
}

.descricao {
    width: 100%;
    height: 100%;

    display: flex;
    flex-direction: column;
    justify-content: center;
}

.descricao .titulo {
    font-size: 64px;
    line-height: 70px;
    
    margin-bottom: 32px;
}

.descricao .titulo-chapeu {
    font-size: 20px;
    line-height: 30px;

    margin-bottom: 24px;
}

.descricao p {
    font-size: 24px;
    line-height: 36px;
    margin-bottom: 32px;
}

.botoes {
    width: 100%;
    height: 52px;
    
    display: flex;
    align-items: center;
    gap: 24px;
}

.botao {
    width: 240px;
    height: 52px;
    border: 1px solid #F1A5B1;
    background-color: transparent;
    color: #fff;
    border-radius: 4px;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 18px;
    font-weight: 700;
    gap: 8px;
}

.botao-primario {
    background-color: #F1A5B1;
    color: #0B0A0A;
}

.ilustracao {
    width: 100%;
    height: 100%;
    background-image: url('../images/image.svg');
    background-repeat: no-repeat;
}

~~~

3. Salve as alterações e feche o arquivo.

## Abrir a página no browser

1. Na bairra de status do VSCode, na parte inferior direita
2. Clique na opção Open Live Server
3. Ele irá abrir a sua página web no navegador.

## Desafio proposto

Faltou fazer a formatação CSS do estado ':hover' dos botões '.link' que estão em '.nav-links' e os botões que estão em '.botoes' e são os '.botao-primario' e '.botao-secundario'.

## Considerações

Nesta aula vimos como criar o projeto completo do Desafio 5 do Studio Ghibli com base no Figma do Projeto. Na próxima aula extra vamos fazer as formatações CSS de responsividade.

Salve Devs, até as próximas!
