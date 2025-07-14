# Taller_herrajes
Proyecto de aplicación web personalizada para digitalizar y automatizar los procesos internos de una empresa de herrajes. La herramienta permite a los usuarios gestionar proyectos, controlar pedidos de artículos fabricados o manipulados (como puertas, soportes, rejillas, etc.), registrar los materiales necesarios y realizar el seguimiento de cada fase de ejecución.

# Tecnologías utilizadas

Backend: PHP 8.2
Frontend: HTML, CSS, JS (clásico con formularios)
Base de Datos: MariaDB (versión 10.4)
Herramientas adicionales: phpMyAdmin, generación de PDF vía script

# Flujo de trabajo

1. Usuarios y Roles
  El sistema admite múltiples tipos de usuario: administrador, oficina, y operario.
  Cada usuario se autentica con nombre y contraseña.
  Los roles determinan los permisos de acceso a funciones específicas (crear proyectos, ver pedidos, editar artículos, etc.).

2. Proyectos
  Un proyecto incluye referencia, fechas de inicio/fin, usuario creador y proveedor asignado.
  Los proyectos pueden tener múltiples pedidos asociados.
  Incluye seguimiento de ejecución mediante una tabla.

3. Pedidos
  Cada pedido está vinculado a un proyecto y contiene:
  Artículo a fabricar o modificar
  Material principal
  Cantidades y dimensiones 
  Estado de trabajo (soldadura, mecanizado, garras, placas)
  Comentarios técnicos
  Se puede generar documentación en PDF de los pedidos .

4. Proveedores
  Los proyectos se vinculan a un proveedor registrado.
  Se almacena nombre comercial, dirección, localidad, código postal y teléfono.

5. Permisos y Seguridad
  Sistema basado en roles y permisos.
  Cada función del sistema está controlada (crear, ver, editar, eliminar).
  Seguridad por autenticación de usuario.
