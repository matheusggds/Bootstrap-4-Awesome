# Bootstrap 4 Init
Stack inicial para um projeto utilizando Bootstrap 4 + SASS + Fonts Awesome

## Editando
Adicione seu proprio css em /sass/theme/_child_theme.scss

Para sobreescrever as variaveis utilize este arquivo
/sass/theme/_child_theme_variables.scss

Por exemplo:
A variavel "$brand-primary" é usada pelo Bootstrap.
Adicione sua propria variavel:
$brand-primary: #ff6600;
em sass/theme/_child_theme_variables.scss para sobreescrever.

## NPM, Gulp, SASS and Browser Sync

### Installing Dependencies
- Tenha certeza de ter Node.js, Gulp, and Browser-Sync [1] instalados globalmente.
- Entao abra seu terminal na pasta raiz do seu projeto
- Run: `npm install` then: `gulp copy-assets`

### Running
Para iniciar e compilar seu SASS, rode em seu terminal:

- `$ gulp watch`

Ou com Browser-sync:

- Primeiro edite as opcoes do browser-sync para referenciar o ambiente do seu projeto no arquivo `/gulpfile.js`:
```javascript
var browserSyncOptions = {
    proxy: "localhost/theme_test/", // <----- CHANGE HERE
    notify: false
};
```

- Entao rode: `$ gulp watch-bs`

[1] Visit [http://browsersync.io](http://browsersync.io) for more information on Browser Sync
