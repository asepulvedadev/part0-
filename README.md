


<h1> Fundamentos de las apliaciones web </h1>
<h2> entrega de los ejercios de la parte 0</h2>
 <p>  primer ejercicio  </p> 
 <h2> 0.4: Nuevo diagrama de nota </h2>
<pre> <code>
 
    sequenceDiagram
    participant browser
    participant server
    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/notes
    activate server
    server-->>browser: HTML document
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
    activate server
    server-->>browser: the css file
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.js
    activate server
    server-->>browser: the JavaScript file
    deactivate server

    Note right of browser: The browser starts executing the JavaScript code that fetches the JSON from the server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/data.json
    activate server
    server-->>browser: [{ "content": "HTML is easy", "date": "2023-1-1" }, ... ]
    deactivate server

    Note right of browser: The browser executes the callback function that renders the note
   </code></pre>

<p> Crea un diagrama similar que describa la situación en la que el usuario crea una nueva nota en la página https://studies.cs.helsinki.fi/exampleapp/notes escribiendo algo en el campo de texto y haciendo clic en el botón Save.

Si es necesario, muestra las operaciones en el navegador o en el servidor como comentarios en el diagrama.

El diagrama no tiene por qué ser un diagrama de secuencia. Cualquier forma sensata de presentar los eventos está bien.

Toda la información necesaria para hacer esto, y los dos ejercicios siguientes, se pueden encontrar en el texto de esta parte. La idea de estos ejercicios es leer el texto una vez más y pensar en lo que está sucediendo allí. No es necesario leer el código de la aplicación pero, por supuesto, es posible. </p>

<h2> 0.5: Diagrama de aplicación de una sola página </h2>
<p> Crea un diagrama que describa la situación en la que el usuario accede a la versión de aplicación de una sola página de la aplicación de notas en https://studies.cs.helsinki.fi/exampleapp/spa. </p>

<h2> 0.6: Nueva nota en diagrama de aplicación de una sola pagina </h2>
<p> Crea un diagrama que represente la situación en la que el usuario crea una nueva nota utilizando la versión de una sola página de la aplicación.

Este fue el último ejercicio, y es hora de enviar tus respuestas a GitHub y marcar los ejercicios como hechos en el sistema de envío de ejercicios. </p>



  
