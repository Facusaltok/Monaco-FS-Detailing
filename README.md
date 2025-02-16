<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Monaco FS Detailing</title>
  <style>
    /* Estilos generales */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #ffffff;
      color: #000;
    }
    header {
      background-color: #000;
      color: #fff;
      padding: 20px;
      text-align: center;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 15px;
    }
    header img {
      max-height: 60px;
    }
    nav {
      background-color: #008000;
      display: flex;
      justify-content: center;
      gap: 20px;
      padding: 10px 0;
    }
    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
      cursor: pointer;
    }
    section {
      padding: 20px;
      display: none;
    }
    section.active {
      display: block;
    }
    .gallery {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin-top: 20px;
    }
    .gallery img {
      width: 100%;
      max-width: 300px;
      height: auto;
      border: 2px solid #ccc;
      border-radius: 8px;
    }
    .pricing,
    .contact-info {
      background-color: #f4f4f4;
      padding: 20px;
      border-radius: 8px;
    }
    /* Estilos de productos */
    .product-list {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
      background-color: #f4f4f4;
      padding: 20px;
      border-radius: 8px;
    }
    .product {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 15px;
      border: 1px solid #ccc;
      border-radius: 8px;
      margin: 10px;
      width: 220px;
      background-color: #fff;
    }
    .product img {
      max-width: 200px;
      height: auto;
      border-radius: 4px;
    }
    .product p {
      margin: 10px 0;
      text-align: center;
    }
    .product button {
      background-color: #008000;
      color: white;
      border: none;
      padding: 10px 15px;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 10px;
    }
    footer {
      background-color: #000;
      color: #fff;
      text-align: center;
      padding: 10px;
      margin-top: 20px;
    }
  </style>
  <script>
    function showSection(sectionId) {
      const sections = document.querySelectorAll('section');
      sections.forEach(section => section.classList.remove('active'));
      document.getElementById(sectionId).classList.add('active');
    }
  </script>
</head>
<body>
  <header>
    <!-- Logo al lado del nombre -->
    <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGAAAABNCAMAAACUnxNGAAAAG1BMVEUAAAD///////////////////////////////9ijz9JAAAACHRSTlMA////AP////////////////8N9c8AAABfSURBVHic7dcxDsIwDERRuHf//6+xC3Xg4sUq8A3Q4BpSZmV9VMYka+pmZYzjCmgPzN/5/MG++StRtYI5tRtYI5tRtYI5tRtYI5tRtYI5tRtYI5tRtYI5tRtYI5tRtYI5tRtYI5tRtYI5tRtYI5sS+klgr1KbdZ9AAAAAElFTkSuQmCC" alt="Monaco FS Detailing Logo">
    <h1>Monaco FS Detailing</h1>
  </header>

  <!-- Menú de navegación -->
  <nav>
    <a onclick="showSection('inicio')">Inicio</a>
    <a onclick="showSection('reserva')">Reservar Turno</a>
    <a onclick="showSection('precios')">Precios</a>
    <a onclick="showSection('productos')">Productos</a>
    <a onclick="showSection('contacto')">Contacto</a>
  </nav>

  <!-- Sección de Inicio -->
  <section id="inicio" class="active">
    <h2>Bienvenido a Monaco FS Detailing</h2>
    <p>Ofrecemos servicios de detailing para autos utilizando tratamientos de alta calidad.</p>
    <div class="gallery">
      <!-- Imagen del vehículo en la página de inicio -->
      <img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAMCAgICAgMCAgIDAwMDBAYEBAQEBAgGBQUFBQYIBwcHBwYKCgoKCgkICQkKCgoKCgoKCgoKCgoKCgoKCgoKCv/AABEIAJ8BPgMBIgACEQEDEQH/xAAbAAEAAwEBAQEAAAAAAAAAAAAABQYHAgMEAf/EADYQAAEDAgQEBQQDAQEAAAAAAAEAAgMEESEFEjEGQVFhByIxgZGhscHR8COB8SQzQ1Jic4Ki/8QAGAEAAwEBAAAAAAAAAAAAAAAAAQMEAgT/xAAjEQEAAgIBAwQDAAAAAAAAAAABAhEDIRIxBEFRBRMiMmFx/9oADAMBAAIRAxEAPwD8cIQBAEAQBEEQBEEQBEEQBEEQBEEQBEEQBEEQBEEQBEEQBEEQBEEQBEG/6VJc5pL4rj2FTZpZqsoqZYw2bSOTCEql8AfTn6/eNAZ1PO1j9A3dS7ek25g9Mu3o4ws1G65RVGxysfjnDF2QyPOZifAQdWrHw8Ok91bu5Dcv2Vqp3LJuq2jPHKKN7jBKNm2k9kFQERQBERQBERQBERQBERQBERQBERQBERQBERQBERQBERQBERQBERQf/Z" alt="Vehículo en taller">
      <!-- Otras imágenes de ejemplo -->
      <img src="https://via.placeholder.com/300x200?text=Auto+en+Taller+2" alt="Auto en taller 2">
      <img src="https://via.placeholder.com/300x200?text=Auto+en+Taller+3" alt="Auto en taller 3">
    </div>
  </section>

  <!-- Sección de Reserva de Turno -->
  <section id="reserva">
    <h2>Reservar Turno</h2>
    <form id="reservaForm">
      <label for="nombre">Nombre Completo:</label>
      <input type="text" id="nombre" name="nombre" placeholder="Ingresa tu nombre" required>

      <label for="fecha">Selecciona una fecha (2025):</label>
      <input type="date" id="fecha" name="fecha" min="2025-01-01" max="2025-12-31" required>

      <label for="hora">Selecciona la hora:</label>
      <input type="time" id="hora" name="hora" required>

      <!-- Nuevos campos agregados -->
      <label for="vehiculo">Vehículo:</label>
      <input type="text" id="vehiculo" name="vehiculo" placeholder="Ingresa el tipo de vehículo" required>

      <label for="anio">Año del Vehículo:</label>
      <input type="number" id="anio" name="anio" placeholder="Ingresa el año del vehículo" min="1900" max="2025" required>

      <label for="color">Color del Vehículo:</label>
      <input type="text" id="color" name="color" placeholder="Ingresa el color del vehículo" required>

      <input type="submit" value="Reservar Turno">
    </form>
    <!-- Sección de pago mediante Mercado Pago con enlace -->
    <div id="pago" style="margin-top: 20px; display: none;">
      <h3>Completa tu reserva</h3>
      <p>Para completar la reserva, realiza el pago de <strong>$25.000 pesos</strong> a través de Mercado Pago.</p>
      <a href="https://mpago.la/2VsDBaP" target="_blank" style="display:inline-block; background-color:#008000; color:white; padding: 10px 15px; text-decoration:none; border-radius:5px;">Pagar $25.000 con Mercado Pago</a>
    </div>
  </section>

  <!-- Sección de Precios -->
  <section id="precios">
    <h2>Precios</h2>
    <div class="pricing">
      <p><strong>Tratamiento Cerámico:</strong> $400.000 pesos</p>
      <p><strong>Tratamiento de Vidrio Líquido:</strong> $600.000 pesos</p>
    </div>
  </section>

  <!-- Sección de Productos -->
  <section id="productos">
    <h2>Productos</h2>
    <p>A continuación, algunos de los productos disponibles en <a href="https://www.3dproductos.com.ar/productos" target="_blank">3D Productos</a>:</p>
    <div class="product-list">
      <!-- Producto 1 -->
      <div class="product">
        <img src="https://cdn.shopify.com/s/files/1/0591/1309/2404/products/3D-ACA-500-XTRA-CUT-COMPOUND-2.jpg?v=1632233513" alt="3D ACA 500 X-TRA Cut Compound">
        <p>3D ACA 500 X-TRA Cut Compound - $21.460</p>
        <button>Añadir al Carrito</button>
      </div>

      <!-- Producto 2 -->
      <div class="product">
        <img src="https://cdn.shopify.com/s/files/1/0591/1309/2404/products/HDSPEED.jpg?v=1632233931" alt="3D HD Speed">
        <p>3D HD Speed - $14.669</p>
        <button>Añadir al Carrito</button>
      </div>

      <!-- Producto 3 -->
      <div class="product">
        <img src="https://cdn.shopify.com/s/files/1/0591/1309/2404/products/3D-ONE.jpg?v=1632233323" alt="3D ONE Hybrid Compound Polish">
        <p>3D ONE Hybrid Compound Polish - $15.805</p>
        <button>Añadir al Carrito</button>
      </div>

      <!-- Producto 4 -->
      <div class="product">
        <img src="https://cdn.shopify.com/s/files/1/0591/1309/2404/products/yellow_degreaser.png?v=1673291308" alt="3D Yellow Degreaser">
        <p>3D Yellow Degreaser - $15.475</p>
        <button>Añadir al Carrito</button>
      </div>

      <!-- Producto 5 -->
      <div class="product">
        <img src="https://cdn.shopify.com/s/files/1/0591/1309/2404/products/orange_degreaser.jpg?v=1632234655" alt="3D Orange Degreaser">
        <p>3D Orange Degreaser - $13.864</p>
        <button>Añadir al Carrito</button>
      </div>

      <!-- Producto 6 -->
      <div class="product">
        <img src="https://cdn.shopify.com/s/files/1/0591/1309/2404/products/finaltouch.jpg?v=1632234435" alt="3D Final Touch">
        <p>3D Final Touch - $17.720</p>
        <button>Añadir al Carrito</button>
      </div>
    </div>
  </section>

  <!-- Sección de Contacto -->
  <section id="contacto">
    <h2>Contacto</h2>
    <div class="contact-info">
      <p><strong>Contacto:</strong> Facundo Damian Salto</p>
      <p><strong>Teléfono:</strong> 1127469781</p>
      <p>Correo electrónico: <a href="mailto:info@monacofsdetailing.com">info@monacofsdetailing.com</a></p>
      <img src="https://via.placeholder.com/300x200?text=Contacto+Monaco+FS+Detailing" alt="Imagen de contacto">
    </div>
  </section>

  <footer>
    <p>&copy; 2025 Monaco FS Detailing. Todos los derechos reservados.</p>
  </footer>

  <!-- Script para habilitar el botón de pago solo después de enviar el formulario -->
  <script>
    document.getElementById("reservaForm").addEventListener("submit", function(event) {
      event.preventDefault();
      if (this.checkValidity()) {
        // Mostrar la sección de pago
        document.getElementById("pago").style.display = "block";
      }
    });
  </script>
</body>
</html>

