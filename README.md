 # MTrek 

Criação de pagina usando o Tailwindcss

 ## Instalação do Tailwindcss CLI

 * Instalar o tailwindcss via NPM via terminal:

    > npm install -D tailwindcss

 * Criando o "tailwind.config.js":
    > npx tailwindcss init

## Configurando o template

* Adicione os caminhos de todos os seus arquivos de modelo no seu arquivo "tailwind.config.js".

    >/** @type {import('tailwindcss').Config} */  
    >module.exports = {  
    >  content: ["./src/**/*.{html,js}"],  
    >  theme: {  
    >    extend: {},  
    >  },  
    >  plugins: [],  
    >}

  
* Adicione as diretivas do Tailwind ao seu CSS

    > @tailwind base;  
    > @tailwind components;  
    > @tailwind utilities;

* Inicie o processo de construção do Tailwind CLI

    > npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch

* Começando a usar o Tailwindcss em seu HTML

    ```    
    <!doctype html>  
    <html>  
        <head>
            <meta charset="UTF-8">
             <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <link href="/dist/output.css" rel="stylesheet">
       </head>
        <body>
            <h1 class="text-3xl font-bold underline">
                Hello world!
            </h1>
        </body>
    </html>
    ```

Para verificação dos comandos css, verifique a documentação do framework [clicando aqui!](https://tailwindcss.com/docs/installation)