# Programming-Basics
Basic course of programming unsing JavaScript with platzi

![Logo](https://static.platzi.com/media/organizations/platzilogo.png)

## ¿Que es HTML/CSS/JS?

Son los tres lenguajes que están en centro para crear sitios web.

![Image 1](https://cdn-images-1.medium.com/max/450/1*pixFq7k28LKsABpDNRCjJw.png)

### HTML

Es un archivo sobre el cual nosotros como programadores trabajamos, dicho lenguaje trabaja conjuntamente con JavaScript y CSS. En HTML tenemos toda la información de nuestro proyecto y la organización de como dicha información es vista por el usuario. Este tambien podría ser un archivo de texto con una extensión diferente (.html). Este es el archivo que realmente interpreta el navegador, es donde se concentran los códigos como HTML o CSS. Todos los archivos de HTML tienen una estructura:

```html
<!DOCTYPE html>
<html lang="es" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Curso de programación Basica</title>
  </head>
  <body>
    <h1 class="header">Hola Mamá estoy aprendiendo</h1>
  </body>
</html>
```

Las etiquetas en verde hacen referencia a la estrucura básica de HTML. Recordar que todos los elementos de HTML deben estar incluidos en alguna etiqueta. Estas etiquetas dependen unicamente de la semantica de la página web La etiqueta `<title></title>` Es una de las más importantes porque [Google](https://www.google.com]) segmetna las páginas gracias a la escritura de la etiqueta title de cualquier página web.

### CSS

En CSS se almacenan todos los diseños y estilos que tienem las páginas web que ya conocemos. Con este lenguaje podemos colocar toda la información atractiva para el usuario. En el siguiente código se agregan algunos estilos escritos en lenguaje CSS (Estilos en cascada). Esta etiqueta de estilos debe estar en la parte del `<head></head>` de la parte de la estructura html como se muestra en el bloque de código acontinuación:

```html
<!DOCTYPE html>
<html lang="es" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Curso de programación Basica</title>
    <style media="screen">
      body{
        background-color: red;
      }
    </style>
  </head>
  <body>
    <h1 class="header">Hola Mamá estoy aprendiendo</h1>
  </body>
</html>
```

Como se puede observar las etiquetas de estilo son: `<style></style>` dichos colores se pueden cambiar con los colores en ingés ó su equivalente hexadecimal.

De igual manera los Indicadores de CSS Cambian respectivamente dependiento del id o de la clase de la etiqueta

### JavaScript

Es el encargado de la interactividad de la página con el usuario en donde los eventos son los causantes de dicha interactividad que se ve reflejada en el navegador. Este es el lenguaje de programación por definición para la web. De igual manera es importante recordar que JavaScript es muy diferente a Java. Java en la actualidad es utilizado por bancos y casas desarrolladoras para crear aplicaciones de escritorio y Js es el lenguaje por definición para la web.

Para agregar directamente javaScript dentro del HTML se utiliza la etiqueta `<script></script>` y dentro de ella se escribe todo el código de JavaScript. Es una buena práctica colocar la etiqueta de JavaScript al final del body como se muestra en el bloque de código acontinuación:

```html
  <body>
    <h1 class="header">Hola Mamá estoy aprendiendo</h1>
   <script type="text/javascript">
    alert("Mensaje especial desde el HTML");
   </script>
  </body>
```


Esta práctca se realiza para que la página cargue completamente y una vez esté cargada empieze la interactividad con el Javascript

## Primeros pasos en el navegador

![Image 2](https://cdn2.iconfinder.com/data/icons/social-media-8/512/Chrome.png)

### Consola

La consola es donde el codigo de Js es leído por el navegador y es donde podemos hacer las pruebas básicas y empezar a jugar con el código.

**Enviar mensaje en consola**: Para enviar mensajes en consola se debe escribir el comando alert. (El punto y coma hace referencia a una buena práctica de programación).

**Declaración de varibles**: la sintaxis en Js para la declaración de variables a diferencia de VBA esta se realiza con la palabra reservada _var_. Dicha declaración siempre se asigna hacia la derecha.

## Programación con JavaScript

Como todo lengiaje de programación JavaScript tiene su propia sintaxis de programación, es [Case Sensitive](https://es.wikipedia.org/wiki/Sensible_a_may%C3%BAsculas_y_min%C3%BAsculas) Lo que significa que el lenguaje diferencia entre mayúsculas y minúsculas.

### Mi peso en otro planeta

Para el primer "mini proyecto" se va a calcular el peso de cada estudiante como si vivieramos en marte. el cual se ejecutó de la siguiente manera:

```html
<!DOCTYPE html>
<html lang="es" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title></title>
  </head>
  <body>
    <h1>Como saber tu peso en marte</h1>
    <script type="text/javascript">
      var peso = prompt("Ingresa tu peso en la tierra");
      var pmarte = (peso * 3.7)/9.8;

      alert("Tu peso en marte es: " + pmarte);
      document.write("No estas pesad@, únicamente estas mal úbicado geograficamente")
    </script>
  </body>
</html>
```

**Nota**: Para controlar el número de cifras significativas de una variable de punto flotante el código es: `nombrevar.toFixed(Número de cifras)` De esta manera 32.568744584 se escribiría en el navegador como 32.56.

Muchas veces a lo largo del desarrollo del código necesitamos información del usuario, un camino para hacerlo sin la necesidad de utilizar formularios es con `prompt("Texto")`. Esto nos ayuda a solicitar la información escrita por el usuario.

Una vez entendio esto se debe aclarar que todos los datos obtenidos por `prompt("texto")` vienen en formato string y si necesitamos volverlos enteros utilizamos el comando `parseInt(prompt("Texto"))`o `parseFloat(prompt("Texto"))`, de esta forma se asegura que si se trabaja con números las operaciones matemáticas sean ejecutadas de la mejor forma posible.
