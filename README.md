# Kit de inicio Webpack
Este kit de inicio esta pensado para todo principiante en webpack y desarrollo Front-End.
Usted puede agregar mas dependencias al proyecto con Angular, React, Vue, y mucho mas. y configurar a su manera a medida que obtenga mas experiencia, el objetivo es ayudar al principiante. 

***author***: Ramon Martinez <ramonmartinezcordero@gmail.com>

***license***: MIT

### Iniciar Kit
  Para Instalar ejecuta **npm install**
  
  Para Iniciar el servidor **npm start**
  Para Iniciar el modo de produccion **npm run build**
  Para Iniciar el modo de desarrollo **npm run dev**

  * **start** : Ejecutar servidor local en modo desarrollo
  * **build**: Empaqueta codigo y genera la carpeta "dist" en modo de producion
  * **dev**: Empaqueta codigo y genera la carpeta "dist" en modo de desarrollo
***

### Estrutura de carpetas 
- dist
- src
    + img
    + js
    + scss
        + main.scss
    + index.js
    + template.html

+ .babelrc 
+ .gitignore
+ .gitconfig
+ package.json
+ postcss.config.js
+ webpack.config.js

### Entradas
+ index.js
+ template.html

**Index.js es el script principal puede trabajar directamente en él o con modulos almacenados en la carpeta js**
### Carpeta dist
  cuando ejecute el comando "build" ó "dev" aqui se genera su empaquetado
  
### Caperta img
deben de ir todas las imagenes de su proyecto
los formatos soportados son: 

+ jpg
+ jpeg
+ gif
+ png
+ webp

agregar mas formatos tendrá que hacerlo en webpack.config.js

### Caperta js
si usted desea trabajar con modulos de JavaScript puede crear sus script en esta carpeta y importarlos a index.js

### Carpeta scss 
en el **main.scss** usted podra trabajar con sass 

### Carpeta css 
en el **main.css** usted podra trabajar con css

### Agregar Multiples entradas HTML

Para agregar otras entradas edite webpack.config.js y agregue en "plugins" el siguiente objeto
```new HtmlWebpackPlugin({

            template: './src/mi nueva-entrada.html',
            inject: true,
            filename: './mi nueva-entrada.html'
            
        })```




 
