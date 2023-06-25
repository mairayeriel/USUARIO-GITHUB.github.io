# Introducción a Git

Hola! Hoy tendremos nuestro primer laboratorio del módulo  **Git y trabajo en equipo**.

Si revisamos el contenido de este repositorio hay un archivo llamado `index.html` que está vacío. Trabajaremos utilizando los comandos aprendidos el el módulo anterior para crear un sitio web.

## Objetivo

Crear, en base a comandos o con VSCode, la siguiente estructura:

```shell
├── portfolio.html
├── about.html
├── index.html
├── README.md
├── test
```

Podemos notar que hay 2 archivos faltantes. Vamos a realizar los pasos necesarios para crearlos y aprender a escribir archivos HTML.

NOTA: El tópico HTML tiene muchos contenidos que por ahora no vamos a profundizar. Vamos a conocer los atajos para crear las estructuras más básicas y en los futuros módulos conoceremos esto en detalle.

## Pre-requisito: Saber escribir un archivo HTML sin saber HTML

Debes escribir los archivos HTML utilizando el atajo utilizando el caractér `!` (signo de exclamación).
Para hacer esto abrimos el archivo `index.html` y hacemos click para escribir contenido. Escribimos el caractér `!` y aparecerá una opción para seleccionar. Una vez seleccionada con la tecla "Enter" o haciendo Clic, aparecerá algo como lo siguiente:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  
</body>
</html>
```

Esta es una estructura HTML básica. Vamos a prestar atención en 2 partes.

La primera denominada `Title` la podemos reconocer ya que está "encerrada" bajo las denominadas "Etiquetas HTML" que es algo como lo siguiente:

```html
<title>Document</title>
```

## Experimentemos con \<title> para entender su utilidad

Vamos a buscar a través de nuestro sistema de archivos (la interfaz visual para navegar por carpetas de nuestro Sistema Operativo) este proyecto.
Al ingresar a la carpeta notarás que el archivo `index.html` tendrá un ícono distintivo del navegador web.
Si hacemos doble clic sobre este se abrirá el navegador y veremos un contenido totalmente en blanco. Pero si ponemos atención veremos que en la pestaña actual veremos el texto "Document".

Volvemos a Visual Studio Code y vamos a modificar el archivo index.html cambando title:

```html
<title>Mi sitio Web</title>
```

Ahora en la ventana del navegador recargamos la pestaña.

¿Qué sucedió?

Exactamente! somos capaces de manipular el texto que se verá en la pestaña del navegador.

Este será nuestro primer acercamiento a HTML. Ahora continuaremos con el contenido que queremos que el usuario vea.

## Escribir información en \<body> con una encabezado de texto y un párrafo

Piensa en los periódicos que buscan mostrar en sus portadas un texto principal que pueda ser visto fácilmente. En los sitios Web sucede algo similar.

Para ello hay una serie de etiquetas HTML que permiten lograr esto y mucho más. Hoy aprenderemos 2 agregando al interior de las etiquetas `<body>` lo siguiente:

```html
  <h1>Página principal</h1>
  <p>En esta página escribiré las características principales sobre mi sitio web</p>
```

Ahora volvamos a la pestaña del navegador, recargamos y listo, ahora veremos lo escrito al interior de Body representado visualmente en el navegador.

Por el momento será todo lo que aprenderemos de HTML.

## Git

Git es la herramienta con la que podemos dejar registro de todo el trabajo que hemos hecho.
Sirve también como una "maquina del tiempo" que nos servirá de guía para recordar lo que hemos hecho durante el tiempo sobre un repositorio de código fuente, es decir, todos los archivos y carpetas que componen un sitio Web, un Software, una aplicación inclusive hasta un Sistema Operativo Completo.

Para entender el sentido más teórico no olvides que puedes encontrar esto en el siguiente link:

[Fundamentos de Git](https://dev-intro-867e7.web.app/docs/git-github/01-fundamentals.html)

En este laboratorio abordaremos la parte práctica de Git aplicando su utilidad para dejar registro del trabajo que hemos hecho.

## Utilizando Git para registrar mi trabajo

**Seleccionar archivos**
```bash
git add index.html
```

**Confirmar y escribir el porque del cambio**
```bash
git commit -m "se agrega contenido para la página index.html"
```

## Actividad

Tu tarea será seguir seleccionando archivos y confirma los cambios de los archivos `about.html` y `portfolio.html` UNO a UNO siguiendo los ejemplos anteriores.

Debes poner un título a través de la etiqueta `<title>` que se corresponda a cada archivo.
También deberás agregar un encabezado y un párrafo a cada uno de estos archivos.


**Termina coordinando los nuevos cambios con la nube de GitHub**

```bash
git push origin main
```

¡Éxito!

## Actividad 2

Agregar links desde el archivo `index.html` hacia `about.html` y `portfolio.html`. Además, estas últimas páginas deben tener un link al `index.html`


El siguiente en un ejemplo que lleva a la página `index.html`
```html
<a href="index.html">Ir al index</a>
```