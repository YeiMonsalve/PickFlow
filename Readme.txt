PickFlow
Sistema de optimización de procesos de picking para almacenes mediante simulación de rutas, asignación de tareas y validación de productos.

Estructura del proyecto
📁 modelos/
Contiene las clases que representan las entidades principales del sistema.

Archivos:

producto.py: información de los productos (SKU, nombre, ubicación).
pedido.py: estructura de los pedidos.
operario.py: datos de los operarios.
ubicacion.py: coordenadas y posiciones dentro del almacén.

📁 servicios/
Contiene la lógica de negocio del proyecto.

Archivos:

rutas.py: calcula rutas de recolección.
picking.py: administra el proceso de picking.
simulador.py: simula dispositivos RFID y localización.
auditoria.py: valida y revisa pedidos completados.

📁 datos/
Almacena los datos utilizados por el sistema.

Archivos:

productos.json: catálogo de productos.
pedidos.json: pedidos pendientes.
operarios.json: listado de operarios.
ubicaciones.json: posiciones del almacén.
Esta información funciona como una base de datos sencilla durante el desarrollo inicial.

📁 plantillas/
Contiene las vistas HTML del sistema.

Archivos:

index.html: página principal.
pedidos.html: gestión de pedidos.
picking.html: interfaz de preparación de pedidos.
auditoria.html: módulo de auditoría.

📁 static/
Contiene los archivos estáticos de la aplicación.

Subcarpetas:

📁 css/
style.css: estilos de la aplicación.
📁 js/
script.js: funciones JavaScript de apoyo para la interfaz.
📁 img/
Imágenes utilizadas por el sistema.
📄 app.py
Punto de entrada principal de la aplicación Flask.

Responsabilidades:

Inicializar el servidor.
Definir las rutas principales.
Conectar vistas y lógica del sistema.
📄 requirements.txt
Lista de librerías necesarias para ejecutar el proyecto.

Ejemplo:

Flask
SQLAlchemy
Bootstrap-Flask
📄 README.md
Documento principal del proyecto.

Contiene:

Descripción general.
Estructura de carpetas.
Instalación.
Ejecución.
Integrantes del proyecto.
Flujo general del sistema
El usuario consulta un pedido.
El sistema identifica los productos requeridos.
Se genera una ruta óptima de recolección.
El operario recorre virtualmente el almacén.
Se valida cada producto seleccionado.
El pedido pasa a auditoría.
El sistema registra estadísticas y resultados.
Integrantes
Yeison Stiven Monsalve López
Yoneibi Dariana Neira Vivas
Kevin Stewart Otálvaro Posada
Miguel Salomón Gil Herrera
Institución
Tecnológico de Antioquia - Institución Universitaria

Ingeniería de Software
2026