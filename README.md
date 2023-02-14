# LINIO STORE REPLICA
La pagina LINIO STORE es una replica de la pagina original Linio, esta pagina fue hecho con tecnologia VTEX.


![image](https://user-images.githubusercontent.com/107804493/218875530-5d771b2a-d58a-49fb-b64f-1d01568038c7.png)


## Configuración
 ### Paso 1 - Configuración Básica 
Para windows 
- Download and install Node.js.
- Download and install Yarn.
- Run the Windows Terminal with elevated administrator permission by right-clicking on the Windows Terminal icon and selecting "Run as administrator.
- Install the VTEX IO CLI by running the following command.
```bash
yarn global add vtex
```
5.Run the following command to complete the installation.
```bash
vtex

```
Documentacion oficial..
https://developers.vtex.com/docs/guides/vtex-io-documentation-vtex-io-cli-install


### Paso 2 - Clonación del repositorio
Clona el repositorio a tu maquina local
![image](https://user-images.githubusercontent.com/107804493/218879370-e022f694-f0ba-4021-84dc-32a1857b5a72.png)

### Paso 3 - Editar el Manifest.json
Deberas editar el campo vendor que se refiere al  cliente que se este trabajando
![image](https://user-images.githubusercontent.com/107804493/218882839-9b795aad-922e-4bf4-92fe-ab4ca37f2a82.png)


### Paso 4 - Instalar apps necesarias
se debe instalar las siguientes aplicaciones 
megamenu
```bash
vtex install vtex.mega-menu@2.x
```
wish list
```bash
vtex install vtex.wish-list
```
question and answers
```bash
vtex install vtex.questions-and-answers@0.x

```

Se debe comprobar las apps instaladas con vtex list 

![image](https://user-images.githubusercontent.com/107804493/218883408-d3e48f6a-7472-4ac6-8b8c-8040facdaeef.png)

Ademas se deben hacer link en las siguientes aplicaciones

![image](https://user-images.githubusercontent.com/107804493/218884205-18ceb4a8-0475-40e8-aa18-cd69c10e9767.png)

### Paso 5 - Desinstalar el store-theme predeterminado
Al entrar por primera vez a la tienda, se tendra un store-theme inicial que debera ser desinstalado
- Ejecutamos vtex list para ver las apps instaladas
- identificamos  vtex.store-theme@0.0.1 y copiamos
- Ejecutamos 
```bash
vtex unistall vtex.store-theme@0.0.1
 ```
### Paso 6 - Ejecute un preview de la tienda
-Una vez ya hayas hecho login y hayas creado tu workspace para ejecutar tu tienda, deberas ejecutar
```bash
vtex link
```
Este permitira sincronizar los archivos de tu computadora con una direccion web que te permitira visualizar la pagina en el navegador.
-Luego ejecutaras 
```bash
vtex browse
```
Este comando sirve para abrir el navegador en la url destinada para visualizar tu tienda


### Dependencies
```bash
"dependencies": {
    "vtex.modal-layout": "0.x",
    "vtex.overlay-layout": "0.x",
    "vtex.store-newsletter": "1.x",
    "vtex.checkout-summary": "0.x",
    "vtex.product-list": "0.x",
    "vtex.store-image": "0.x",
    "vtex.store": "2.x",
    "vtex.store-header": "2.x",
    "vtex.product-summary": "2.x",
    "vtex.store-footer": "2.x",
    "vtex.store-icons": "0.x",
    "vtex.store-components": "3.x",
    "vtex.disclosure-layout": "1.x",
    "vtex.styleguide": "9.x",
    "vtex.slider": "0.x",
    "vtex.carousel": "2.x",
    "vtex.shelf": "1.x",
    "vtex.menu": "2.x",
    "vtex.minicart": "2.x",
    "vtex.product-details": "1.x",
    "vtex.product-kit": "1.x",
    "vtex.search-result": "3.x",
    "vtex.login": "2.x",
    "vtex.my-account": "1.x",
    "vtex.flex-layout": "0.x",
    "vtex.rich-text": "0.x",
    "vtex.store-drawer": "0.x",
    "vtex.locale-switcher": "0.x",
    "vtex.product-quantity": "1.x",
    "vtex.product-identifier": "0.x",
    "vtex.product-specification-badges": "0.x",
    "vtex.product-review-interfaces": "1.x",
    "vtex.telemarketing": "2.x",
    "vtex.order-placed": "2.x",
    "vtex.stack-layout": "0.x",
    "vtex.tab-layout": "0.x",
    "vtex.responsive-layout": "0.x",
    "vtex.slider-layout": "0.x",
    "vtex.iframe": "0.x",
    "vtex.breadcrumb": "1.x",
    "vtex.sticky-layout": "0.x",
    "vtex.add-to-cart-button": "0.x",
    "vtex.category-menu": "2.x",
    "vtex.search": "2.x",
    "vtex.product-price": "1.x",
    "vtex.product-availability": "0.x",
    "vtex.css-handles": "0.x",
    "vtex.toggle-layout": "0.x",
    "vtex.store-link": "0.x",
    "vtex.product-specifications": "1.x"

  },
```
```bash
 "peerDependencies": {
    "vtex.mega-menu": "2.x",
    "vtex.wish-list": "1.x",
    "vtex.questions-and-answers": "0.x"
  },
```

### Custom Apps (Componentes custom que deben instalarse con la tienda)
```bash
    "itgloberspartnercl.whatsapp-button": "0.x",
    "itgloberspartnercl.bullets-diagramation": "0.x",
    "itgloberspartnercl.add-to-cart-info": "0.x",
    "itgloberspartnercl.custom-department-search": "0.x",
    "itgloberspartnercl.pdf-reader": "0.x",
    "itgloberspartnercl.quick-order": "0.x",
    "itgloberspartnercl.special-diagramation": "0.x"
```
### Contributors
1. MAICOL ALEXIZ ORITZ HERNANDEZ
2. Desde forma indirecta con sus consejos y recomendaciones, mis tutores Luis Felipe Cerero García, David Mosquera y Julio César Arroyave 

