
<html> 
 <head>
<style>
    body {
      font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      margin: 2rem;
      background: #f9f9f9;
      color: #333;
    }

    h1, h2, h3 {
      color: #2c3e50;
    }

    pre {
      background: #272822;
      color: #f8f8f2;
      padding: 1em;
      border-radius: 8px;
      overflow-x: auto;
    }

    code {
      font-family: Consolas, monospace;
      font-size: 0.95em;
    }

    p code {
      background: #eaeaea;
      padding: 0.2em 0.4em;
      border-radius: 4px;
    }

    hr {
      margin: 2rem 0;
    }
  </style>

 
 </head>
 <body>
<h1> Fundamentos de las apliaciones web </h1>
<h2> entrega de los ejercios de la parte 0</h2>
 <p>  primer ejercicio  </p> 
<p><code> 
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

    Note right of browser: The browser executes the callback function that renders the notes


</code></p>

<p> Crea un diagrama similar que describa la situación en la que el usuario crea una nueva nota en la página https://studies.cs.helsinki.fi/exampleapp/notes escribiendo algo en el campo de texto y haciendo clic en el botón Save.

Si es necesario, muestra las operaciones en el navegador o en el servidor como comentarios en el diagrama.

El diagrama no tiene por qué ser un diagrama de secuencia. Cualquier forma sensata de presentar los eventos está bien.

Toda la información necesaria para hacer esto, y los dos ejercicios siguientes, se pueden encontrar en el texto de esta parte. La idea de estos ejercicios es leer el texto una vez más y pensar en lo que está sucediendo allí. No es necesario leer el código de la aplicación pero, por supuesto, es posible. </p>
</body>
</html>

  
