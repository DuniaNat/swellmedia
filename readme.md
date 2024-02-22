# Como empezar a compilar con SCSS

1. Abrir la consola en esta carpeta de backup o nueva con ctrl+ñ
    a. npm install nodemon node-sass
    b. npm init // Metralleta de enter (11 enters)

2. Abrir el archivo package.json y editarlo
    a. A continuación de && exit 1" colocar una , presionar enter
    y pegar el siguiente texto:

"build-css": "node-sass --include-path scss scss/main.scss css/style.css",
"watch-css": "nodemon -e scss -x \"npm run build-css\""

3. Crear las carpetas con sus respectivos archivos
    a. scss/main.scss
    b. css/style.css

4. En la consola correr el comando
    a. npm run build-css // Por única vez
    b. npm run watch-css      

5. Cada vez que se quiera seguir compilando en SASS
    a. abrir la consola con ctrl+ñ
    b. npm run watch-css

//FIN  