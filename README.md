# Proyecto de Pruebas Automatizadas con Selenium WebDriver en C#

## 1. Descripción General del Proyecto

El objetivo de este proyecto es automatizar las pruebas de una aplicación o página web (desarrollada por el estudiante o ya existente) usando **Selenium WebDriver en C#**.  
La prueba automatizada valida diferentes escenarios de la aplicación, genera capturas de pantalla de forma automática y crea un reporte en formato HTML con los resultados obtenidos.  
El proyecto se entrega a través de plataformas como **Azure DevOps** o **GitHub**, acompañado de un video demostrativo de la ejecución de las pruebas.

## 2. Requisitos Técnicos

### 2.1. Selenium WebDriver
- Utilizar **Selenium WebDriver** para interactuar con la aplicación web.
- Descargar e integrar el controlador (driver) del navegador (por ejemplo, **ChromeDriver** para Google Chrome).

### 2.2. Entorno de Desarrollo en C#
- Utilizar **Visual Studio** o **Visual Studio Code** con la extensión de C#.
- Crear un proyecto de tipo Consola (puede ser .NET Core o .NET Framework).

### 2.3. Funcionalidades de la Prueba
Las pruebas deben:
- Validar diferentes escenarios de la aplicación.
- Generar capturas de pantalla automáticamente durante la ejecución de las pruebas.
- Crear un reporte en formato **HTML** con los resultados obtenidos.

## 3. Historias de Usuario

### Historia de Usuario 1: Inicio de Sesión Exitoso
- **Como usuario registrado**, quiero ingresar a la aplicación mediante mis credenciales, para acceder a mi perfil y datos personales.
- **Criterios de Aceptación:**
  - Se ingresan credenciales válidas.
  - Al hacer clic en “Iniciar Sesión”, se redirige al usuario a su página de perfil.
  - Se muestra un mensaje de bienvenida o se visualiza un elemento identificador (por ejemplo, un div con el ID `perfilUsuario`).
- **Criterios de Rechazo:**
  - Las credenciales inválidas muestran un mensaje de error.
  - El sistema no permite el acceso sin autenticación.

### Historia de Usuario 2: Registro de Nuevo Usuario
- **Como nuevo usuario**, quiero registrarme en la aplicación ingresando mis datos personales, para acceder a funciones exclusivas para usuarios registrados.
- **Criterios de Aceptación:**
  - El formulario solicita datos obligatorios: nombre, correo y contraseña.
  - Se valida el formato del correo y la fortaleza de la contraseña.
  - Al enviar el formulario, se crea la cuenta y se muestra una página de confirmación.
- **Criterios de Rechazo:**
  - Campos vacíos o con datos incorrectos disparan mensajes de error.
  - El sistema no crea la cuenta si los datos no cumplen los requisitos mínimos.

### Historia de Usuario 3: Búsqueda de Productos
- **Como usuario**, quiero buscar productos por palabras clave, para encontrar rápidamente lo que necesito.
- **Criterios de Aceptación:**
  - La barra de búsqueda acepta texto y, al presionar “Buscar”, se muestran productos relevantes.
  - Los resultados incluyen imagen, nombre y precio.
- **Criterios de Rechazo:**
  - Si la búsqueda no devuelve resultados, se muestra un mensaje “No se encontraron productos”.
  - No se permite la inyección de código malicioso.

### Historia de Usuario 4: Agregar Producto al Carrito
- **Como usuario**, quiero agregar un producto a mi carrito, para proceder con la compra.
- **Criterios de Aceptación:**
  - Al presionar “Agregar al carrito”, el producto aparece en el resumen del carrito.
  - Se actualiza el contador en el ícono del carrito.
- **Criterios de Rechazo:**
  - Si el producto no tiene stock, se muestra un mensaje informativo y no se agrega.

### Historia de Usuario 5: Proceso de Pago
- **Como usuario**, quiero finalizar el proceso de pago, para completar mi compra de manera segura.
- **Criterios de Aceptación:**
  - Se selecciona el método de pago (tarjeta, PayPal, etc.).
  - Después de la validación, se muestra una página de confirmación de compra.
  - Se envía un correo electrónico confirmando la transacción.
- **Criterios de Rechazo:**
  - En caso de error en el pago, se muestra un mensaje con información del fallo.
  - La transacción no se realiza sin la validación adecuada.

## 4. Capturas de la Implementación del Proyecto

La aplicación web está desarrollada utilizando **HTML, CSS y JavaScript**, implementando un CRUD para gestionar la información de los usuarios y productos.  
Se han incluido capturas en los siguientes momentos clave:

- **Gestión de Búsqueda:** Muestra la funcionalidad en la que el usuario realiza una búsqueda y se presentan los resultados de productos.
- **Antes de Someter el Pago:** Visualización de la interfaz donde se revisa el contenido del carrito y se prepara la transacción.
- **Cuando el Usuario Genera el Pago:** Captura de la confirmación de pago y la generación del reporte de resultados.

> **Nota:** Las capturas de pantalla se encuentran en la carpeta `Capturas/` dentro del repositorio y también se incluyen en el reporte HTML generado tras la ejecución de las pruebas.

## 5. Ejecución y Reporte

- **Ejecución de Pruebas:**  
  Las pruebas se ejecutan utilizando Selenium WebDriver en conjunto con pruebas unitarias en C#.  
  Al finalizar, se genera un reporte en formato HTML donde se resumen los resultados, se incluyen capturas de pantalla y se detalla el estado de cada historia de usuario.

- **Entrega:**  
  El proyecto se entrega en plataformas como **Azure DevOps** o **GitHub** junto con un video demostrativo en el que se muestra la ejecución completa de las pruebas automatizadas.

## 6. Contribuciones

Las contribuciones son bienvenidas. Si deseas colaborar:
- Realiza un fork del repositorio.
- Crea una rama para tus mejoras o correcciones.
- Envía un pull request para revisión.

## 7. Licencia

Este proyecto se distribuye bajo la [Licencia MIT](LICENSE).

