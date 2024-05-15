## <h1>Application Angular 17 Web Component </h1>
***
<table>
  <tr>
    <td><img src="https://www.mag-corp.com/wp-content/uploads/2021/08/angular.png" alt="drawing" height="260px"/></td>
  </tr>
</table>

## Informations Générales
***
Mise en place d'un WebComponent version 17 <br>
```
$ ng build
$ ng serve
```
La build commande permet de génerer des fichier dans le repertoir destination dist/browser

Creer à la racine du projet le fichier vite.config.js
```
import { defineConfig } from "vite";

export default defineConfig({
    build: {
        rollupOptions: {
            output: {
                entryFileNames: "[name].js"
            },
            input: "build.js"
        },
        outDir: "./dist/widget"
    }
});
```
Modifier le fichier package.json
```
"scripts": {
  "build:vite": "ng build --output-hashing=none --configuration=production && vite build",
  },
```
Lancer la commande
```
npm run build:vite
```
Un fichier build.js pret à être integre sous forme de WebComponent

## Technologies
***
Technologies utilisées:
* Angular 17 JS
  
## Instalation
***
Voir ci-dessus

## FAQs
***
Quelques lignes de commandes utiles<br>
```
Désinstaller la version courante
npm uninstall -g @angular/cli

Installer la version
npm install -g @angular/cli@17

```

