# guia de PC

Iniciamos el project con NPM
    descargamos NodeJS
    descargamos NPM

Configuramos el servidor
    npm init
        -name: name_project
        -version: (default)
        -description: description the project de NodeJS
        -entry point: <index.html>
        -test command: none (enter)
        -git repository: (default)
        -keyboards: none (default)
        -author: name
        -license: (default)
        [create package.json]
        -yes

Definir nuestro servidor web
(git commit) : "definimos el package.json"

    we user the library LITE-SERVER [npm]
        ```bash
        npm install lite-server --save-dev
        ```

    we edit the package.json 
    added
        ```json
            "scripts":{
                "dev": "lite-server",
              },
        ```
    we execute 
        ```npm run dev```

Para dejar de hacer commit una carpeta
    creamos la carpeta .gitignore
        ```git
        node_modules
        ```
    ahora al hacer commit ignora la carpeta node_modules 

    git commit "added lite-server"


We Add package
    bootstrap
        ```bash 
            npm install bootstrap --save
            npm install jquery --save 
            npm install popper.js --save 
        ```
    CONFIGURAMOS INDEX.HTML 
        ```html 
            <head>
                <!--Bootstrap CSS-->
                <link href="node_modules/bootstrap/dist/css/bootstrap.min.css">
            </head>
            <body>
                <script src="node_modules/jquery/dist/jquery.min/js">
                <script src="node_modules/popper.js/dist/popper.min.js">
                <script src="node_modules/bootstrap/dist/js/bootstrap.min/js">
            </body>
        ```
        git commit -m "we include in the HTML file bootstrap, jquery, popper"

