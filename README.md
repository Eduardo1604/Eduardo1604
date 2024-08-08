<body>
    <h1>¿Me perdonas amorcito 😿?</h1>
    <div class="button-container">
        <button class="button" id="si-button" onclick="respuesta('si')">Sí</button>
        <button class="button" id="no-button" onclick="respuesta('no')">No</button>
    </div>

    <script>
        function respuesta(respuesta) {
            if (respuesta === 'si') {
                alert(gracias mi vida te amo mucho );
            } else {
                alert(bueno:) nojaooo');
            }
        }
        setInterval(moverBotonNoAleatoriamente, 500);

        function moverBotonNoAleatoriamente() {
            var botonNo = document.getElementById('no-button');
            var maxX = window.innerWidth - botonNo.offsetWidth;
            var maxY = window.innerHeight - botonNo.offsetHeight;

            var randomX = Math.floor(Math.random() * maxX);
            var randomY = Math.floor(Math.random() * maxY);

            botonNo.style.position = 'absolute';
            botonNo.style.left = randomX + 'px';
            botonNo.style.top = randomY + 'px';
        }
    </script>
</body>
