# Prueba Técnica MOVISAT.

En este documento se indicará los pasos a seguir para poder utilizar la librería creada.
Para utilizar los componentes se deben primero que todo importar en el app.component.ts principal de tu proyecto, por lo general es en src/app/

![image](https://github.com/Lack01/geekforgeeks/assets/83151093/0dc363d3-0122-4d36-95b8-92d8cf0dbbf2)

## Importación de componentes

Los 3 principales componentes de esta librería son estos que dejo subrayado en verde.

![image](https://github.com/Lack01/geekforgeeks/assets/83151093/32957f25-81d7-407e-9433-523df3e997d1)

## Archivo HTML

Una vez importados, se debe dirigir al archivo .html principal, en este caso siendo un proyecto común sería:

![image](https://github.com/Lack01/geekforgeeks/assets/83151093/cfc6d3a4-5ef2-4001-bdbe-166cf3a2599b)

El archivo app.component.html que se encuentra en la misma carpeta del archivo donde realizamos la importación de los componentes.
Una vez dentro del archivo .html se debe seguir con la estructura que se muestra a continuación:

```
<div class="container">
  <ngx-parent></ngx-parent>         <!--componente de parent donde va la card con el texto --> 
  <div class="button-container">
    <ngx-void-button                     
      [text]="'Cancelar'"
      [btnClass]="'btn btn-secondary'"
      ></ngx-void-button>                <!--primer botón de cancelar, sólo se le cambia el text y la class --> 
      <ngx-void-button
      [text]="'Aceptar'"
      [btnClass]="'btn btn-primary'"
    ></ngx-void-button>                  <!--segundo botón reutilizable con propiedades distintas --> 
    <ngx-void-button
      [text]="'Abrir Modal'"
      [btnClass]="'btn btn-success'"
      data-bs-toggle="modal"
      data-bs-target="#exampleModal"
    ></ngx-void-button>                 <!--Tercer botón --> 
  </div>
</div>

<ngx-modal></ngx-modal>                <!--Componente modal --> 

```

## Muestra

Si existe otro contenido en este archivo borrarlo por completo, reemplazándolo por el de la imagen.

Una vez realizado el paso anterior te deberá aparecer algo así:

![image](https://github.com/Lack01/geekforgeeks/assets/83151093/3d223d8b-0ede-434d-b9b9-9e28872cd56d)

Donde el único botón que realiza una acción sería el “Abrir Modal”:

![image](https://github.com/Lack01/geekforgeeks/assets/83151093/d18739ad-74de-43fb-bd30-5c7f0524b173)

Que muestra una modal de ejemplo para poder modificar a gusto 👌.






