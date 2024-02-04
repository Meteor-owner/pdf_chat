<template>
    <div class="container">
        <header>
            <div id="logo">Real-Time PDF Reader</div>
            <!-- Add any additional header elements here -->
        </header>

        <main>
            <div id="pdf-viewer">
                <!-- PDF.js will render the PDF here -->
                <canvas id="pdf-canvas">
                    <a href="https://www.adobe.com/content/dam/acom/en/devnet/acrobat/pdfs/pdf_open_parameters.pdf"></a>

                </canvas>
                <div id="page-controls">
                    <button id="prev-page">Previous Page</button>
                    <span id="page-num"></span>
                    <button id="next-page">Next Page</button>
                </div>
            </div>
            <aside id="sidebar">
                <div id="chat">
                    <div id="chat-messages">
                        <!-- Real-time chat messages will appear here -->
                    </div>
                    <input type="text" id="chat-input" placeholder="Enter your message...">
                    <button id="send-message">Send</button>
                </div>
                <!-- Add any additional sidebar elements here -->
            </aside>
        </main>
        <footer>
            <span>&copy; 2023 Real-Time PDF Reader</span>
            Add any additional footer elements here
        </footer>
    </div>
</template>

<script>

export default {
    name: 'HomeView',
    components: {
    }
}
</script>


<style scoped>
/* styles.css */
.container {
    height: 100%;
    margin: 0;
    font-family: 'Arial', sans-serif;
    background: #f7f7f7;
}

header {
    background: #333;
    color: #fff;
    padding: 10px 20px;
    text-align: center;
}

main {
    display: grid;
    grid-template-columns: 3fr 1fr;
    height: calc(100% - 60px);
    gap: 10px;
    padding: 10px;
}

#pdf-viewer {
    background: #fff;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding: 20px;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

canvas#pdf-canvas {
    width: 100%;
    border: 1px solid #ddd;
}

#page-controls {
    margin-top: 10px;
}

aside#sidebar {
    display: flex;
    flex-direction: column;
    gap: 10px;
}

#chat {
    background: #fff;
    padding: 10px;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    flex-grow: 1;
    display: flex;
    flex-direction: column;
}

#chat-messages {
    flex-grow: 1;
    overflow-y: auto;
}

#chat-input {
    border: 1px solid #ddd;
    padding: 5px;
    border-radius: 3px;
    margin-top: 10px;
}

#send-message {
    background: #5cb85c;
    color: white;
    border: none;
    padding: 10px 20px;
    margin-top: 5px;
    border-radius: 3px;
    cursor: pointer;
}

#send-message:hover {
    background: #4cae4c;
}

footer {
    background: #333;
    color: #fff;
    text-align: center;
    padding: 10px 20px;
    position: fixed;
    bottom: 0;
    width: 100%;
}
</style>