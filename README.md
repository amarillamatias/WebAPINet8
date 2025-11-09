# WebAPINet8

## Descripción General
WebAPINet8 es una API REST desarrollada en .NET 8 para la gestión de clientes y archivos asociados, con registro de eventos y errores. Permite registrar clientes con fotografías, cargar múltiples archivos comprimidos (ZIP) asociados a cada cliente, y realizar seguimiento de errores mediante un log centralizado. Incluye endpoints para la consulta y administración de los datos registrados.

## Funcionalidades Principales
- **Registro de Clientes:** Permite registrar clientes con información básica y hasta tres fotografías de su vivienda.
- **Carga de Archivos:** Permite subir archivos comprimidos (.zip) asociados a un cliente, descomprimirlos, almacenarlos en el servidor y registrar sus datos en la base de datos.
- **Seguimiento y Registro de Errores:** Captura automáticamente excepciones y eventos relevantes en la API, almacenándolos en la tabla `LogApi`.
- **Consulta de Logs:** Endpoint para consultar los registros de errores y eventos.
- **Documentación interactiva:** Integración con Swagger para probar y explorar los endpoints de la API.

## Tecnologías Utilizadas
- .NET 8
- ASP.NET Core Web API
- Entity Framework Core
- SQL Server
- Swashbuckle (Swagger)

## Estructura del Proyecto
- `Controllers/` - Controladores de la API (Clientes, Archivos, Logs)
- `Models/` - Entidades del dominio (`Cliente`, `ArchivoCliente`, `LogApi`)
- `Data/` - Contexto de base de datos (`ApplicationDbContext`)
- `Middleware/` - Middleware para registro de errores
- `Program.cs` - Configuración principal de la aplicación

## Instrucciones de Ejecución Local

1. **Clonar el repositorio:**# WebAPINet8
