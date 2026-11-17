# Showroom by Gallego Projects · Portal de briefings

Versión de prueba funcional. Dos recorridos reutilizables: interiorismo y reforma integral. No contiene datos del cliente Antonio ni planos privados.

## Estado comprobado
- Navegación completa de ambos formularios en navegador de escritorio.
- Campos, selección de estilo y domótica, conservación entre pasos y datos de contacto entre recorridos.
- Descarga real de ambos PDF; extracción de texto verificada.
- Selección de archivo y descarga de ZIP con PDF, JSON y archivo original verificada.
- Web Share con archivo cuando el dispositivo lo admite; alternativa de descarga manual. Envío real por WhatsApp pendiente de prueba en móvil.
- Responsive implementado; prueba en dispositivo móvil pendiente.

## Pendiente para producción
1. Conectar un repositorio GitHub con permisos de escritura; actualmente la conexión no tiene instalaciones ni repositorios accesibles.
2. Publicar dist en GitHub Pages (rama main, directorio /docs si se renombra dist a docs, o flujo Actions de despliegue).
3. Conectar un servicio de recepción y correo, con credenciales exclusivamente en servidor; GitHub Pages solo aloja la web estática.
4. Configurar remitente autorizado, destinatario fijo showroom@gallegoprojects.es y copia al correo verificado del cliente. No introducir claves de correo en JavaScript público.
5. Integrar protección antiabuso, límites y validación de adjuntos en servidor, almacenamiento privado y política de conservación. Servir PDF/adjuntos mediante enlaces privados temporales cuando excedan el tamaño del correo.
6. Incorporar aviso de privacidad definitivo de la sociedad responsable y texto de entrega. El prototipo no sube ni envía información.
7. Prueba de recepción real en ambas bandejas, PDF, adjuntos, errores, reintentos sin duplicados y móvil. No declarar envío realizado hasta confirmación del servicio.
8. Configurar dominio corporativo mediante DNS si se desea. No se ha creado ni reservado un dominio.

## Prueba sin instalación
Abrir Showroom_Briefings_Prueba.html en un navegador completo. Es un archivo autónomo con imágenes y dependencias incorporadas. Para el despliegue usar dist, que separa archivos.

## Datos
Las respuestas permanecen en memoria hasta cerrar; guardar borrador es opcional en localStorage de este navegador. Adjuntos solo en memoria, no se conservan al cerrar. PDF incluye listado de archivos; ZIP incluye originales. Las referencias de inspiración se identifican como generadas con IA. Se requiere revisión final de accesibilidad, compatibilidad móvil y aviso de privacidad antes de producción.

## Dependencias
jsPDF 3.0.4 (MIT) y JSZip 3.10.1 (MIT o GPLv3), distribuciones con avisos de licencia incorporados. Assets originales del showroom y tablero de inspiración creado para este proyecto.
