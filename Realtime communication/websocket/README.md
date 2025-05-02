- Install dependencies

    ```bash
    npm install
    ```

- Run local server 

    ```bash
    node server.js
    ```

- Open browser console and run the following code to test the WebSocket connection:

    - First step
        ```javascript
        const socket = new WebSocket('ws://localhost:3000');
        console.log(socket);
        socket.onmessage = (e) => console.log(e.data);
        ````

    - Second step

        ```javascript
        socket.send('Hello from client');
        ```

- [MDN Doc](https://developer.mozilla.org/en-US/docs/Web/API/WebSocket)