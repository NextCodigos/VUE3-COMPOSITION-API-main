# VUE3-COMPOSITION-API

Ejemplo de Interacción entre Componentes Padre-Hijo en Vue.js

Este repositorio contiene una aplicación simple en Vue.js que demuestra la interacción entre componentes padre-hijo utilizando props, eventos y el mecanismo provide / inject.
Componentes
App.vue

El componente principal que actúa como el padre de los componentes hijos.

    La plantilla incluye un título para el padre, un componente hijo HijoVue y otro componente hijo HijoVue2.
    El padre proporciona datos (nombre y edad) y un canal (miCanal) a sus componentes hijos.
    Se define un método cambiarValor para modificar los valores de nombre y edad.

Hijo.vue

Un componente hijo que recibe props y emite un evento para modificar datos en el componente padre.

    Muestra las props recibidas nombre y edad.
    Proporciona un botón que activa el método enviar, el cual emite un evento modificar al padre con nuevos valores.

Hijo2.vue

Otro componente hijo que accede a datos proporcionados por el componente padre mediante el mecanismo inject.

    Muestra el valor del canal inyectado.
    Proporciona un botón que activa el método modificar, cambiando el valor de canal.

Cómo Ejecutar

    Clona este repositorio: git clone <repository_url>
    Navega a la carpeta del proyecto: cd <repository_folder>
    Instala las dependencias: npm install o yarn install
    Ejecuta el servidor de desarrollo: npm run serve o yarn serve
    Abre tu navegador y ve a http://localhost:8080 para ver la aplicación en acción.

¡Siéntete libre de explorar y modificar los componentes para aprender más sobre las interacciones entre padres e hijos en Vue.js!

App2.vue:

Ejemplo de Manipulación Dinámica de Datos en Vue.js

Este archivo (App2.vue) presenta ejemplos de cómo manejar datos dinámicos en una aplicación Vue.js.
Contenido del Componente

El componente muestra cómo trabajar con datos y directivas Vue.js para lograr una manipulación dinámica de la interfaz de usuario.

    El nombre dinámico es: {{ name.toLocaleUpperCase() }}

    Un título que cambia el color en función de la propiedad styleColor.

    Un ejemplo de cambio de color basado en un array de colores usando :style.

    El estado "activo" se maneja utilizando un operador ternario para mostrar diferentes mensajes.

    Se muestra el contenido del array arrayColores.

    Los elementos HTML se muestran condicionalmente utilizando v-if, v-else-if y v-else.

    Un elemento se muestra u oculta usando la directiva v-show.

    El contenido del array arryFrutas se presenta tanto de forma procedural como con un ciclo v-for.

Cómo Ejecutar

    Asegúrate de tener un entorno configurado con Vue.js.
    Copia el contenido del archivo App2.vue.
    Pega el contenido en un componente Vue llamado App2.vue en tu proyecto.
    Asegúrate de que el componente esté correctamente importado y configurado en tu aplicación Vue.
    Observa cómo los datos cambian dinámicamente en función de las propiedades y directivas de Vue.js.

Siéntete libre de experimentar con el código y modificar los valores para explorar aún más la manipulación dinámica de datos en Vue.js.

