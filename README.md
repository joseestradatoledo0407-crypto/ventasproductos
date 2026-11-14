# SuperProductos

Tienda web de accesorios de cómputo para San Isidro, Lima. Está hecha con HTML, CSS y JavaScript sin frameworks ni proceso de compilación.

## Ejecutar

Abre `index.html` en un navegador o sírvelo desde cualquier servidor estático. El catálogo de demostración permite explorar la interfaz; para leer y guardar datos reales, pulsa el engranaje de conexión e ingresa la URL y la clave pública (publishable/anon) del proyecto Supabase.

La configuración inicial usa el proyecto `rxrilbqxiolyocfjpruj` y las tablas `producto`, `vendedor` y `ventas`. La clave se mantiene solo en `sessionStorage` del navegador. No uses una clave `service_role` en esta aplicación cliente.

## Esquema de ventas

La aplicación carga productos y vendedores desde sus tablas. Al grabar, inserta una fila por cada producto del carrito en `ventas`, con vendedor, producto, cantidad, precio unitario y total de línea. En el engranaje se pueden ajustar los nombres de las tablas y columnas para que coincidan con el esquema real.

Los nombres de columnas comunes en español se detectan automáticamente. Si tu tabla requiere columnas adicionales, una estructura distinta (por ejemplo, cabecera y detalle) o autenticación por vendedor, el guardado debe adaptarse a ese esquema. La clave pública necesita permisos de lectura para `producto` y `vendedor`, e inserción para `ventas`, con políticas RLS apropiadas.

## Contacto

- San Isidro, Lima
- Teléfono y WhatsApp: +51 943 094 835
- Correo: joseestradatoledo0407@gmail.com
