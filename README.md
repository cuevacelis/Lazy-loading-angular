# Lazy Loading Angular

Este proyecto fue generado con [Angular CLI](https://github.com/angular/angular-cli) version 9.1.0.

## Install
1. git clone https://github.com/cuevacelis/Lazy-loading-angular.git
2. npm install

## Description

Ejemplo construido con Lazy-loading o carga perezosa<br />
1. Acelera la carga inicial de tu Pagina Web.
2. Llama a los componentes que necesitas, cuando los necesitas.

## ¿Problema?

Al visitar una pagina Web construida en Angular, esta llama a AppModule en donde estan listados todos tus componentes.
Lo cual representa en un llamado a todos los componentes declarados en tu aplicacion.<br />
Supongamos que tenemos en nuestra aplicacion dos vistas "Clientes" y "Operarios".<br />
Pero solo necesitamos acceder a la vista de Clientes para visualizar la informacion de uno de ellos.<br />
Entonces ¿Por que la pagina web necesitaria tambien cargar "Operarios" si nunca lo vamos a usar?, haciendo un tiempo inicial de espera mucho mas largo, cargando un componente innecesario para nosotros.

## Solución
Al usar Lazy Loading en la carga incial cargariamos a los componentes que vamos a necesitar

## Conlusión
Entonces es ¿Lazy Loading necesario en todos los proyectos?.
La respuesta es depende del tamaño del proyecto, si tienes un proyecto pequeño quizas no te convenga usar lazy loading, puesto que al hacer la carga incial cargara todos los componentes, lo cual resulta que la interaccion entre ellos sera mas rapida, puesto que ya todos los componentes fueron cargados y no se neceitara volver a llamarlos :)
