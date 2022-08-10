# Documentación

Creación de un *nuevo Theme* para la web de España de Global Exchange.

## Guía de estilo

Anexada al proyecto se incluye una pequeña guía de estilo para la codificación de una hoja de estilo uniforme de la aplicación.

## Proceso

Ante la complejidad de visualizar los cambios realizados en la maquetación de la web a través de los módulos de la aplicación en DNN y las soluciones en Visual Studio, se ha optado por crear en VS Code una réplica de la estructura de cada página y aplicarle el *nuevo Theme* para poder visualizar los cambios en vivo y agilizar el proceso de codificación.

### DNN

- Inserción de las imágenes del prototipo
- Actualización de componentes para adaptar el contenido de la web al contenido del prototipo (añadir, modificar o eliminar elementos).

### VS Code

- Montar entorno de desarrollo
- Aplicar estructura original de las páginas que conforman la web
- Extracción de estilos del prototipo
    - Tipografía
    - Colores
- Extracción de imágenes e iconos del prototipo
- Estilizado de componentes básicos (botones, selectores, campos de formulario...)
- Estilizado del resto de componentes
- Estilizado de cada página de la web en todos los dispositivos
- Testing

### Visual Studio

- Montar entorno de preproducción
- Una vez finalizada la codificación de cada página se probará en el entorno de preproducción montado

## Prototipo

El prototipo se puede visualizar en la siguiente dirección *[Prototipo](https://app.zeplin.io/project/62d5081e64a4a113cbcd1151)*.
Si no se poseen permisos de visualización en la carpeta `prototipes` se incluyen las capturas del mismo.

## Estilos

La codificación de estilos de la página original se extraen del archivo `skin.css`.
El código de este archivo es el que se sustituirá por el nuevo incluido en `style.css` para aplicar los nuevos estilos.
Para probar los nuevos cambios, en Visual Studio se recompilará el módulo asociado a dicho archivo y posteriormente se llevará el código a la aplicación copiando y pegando la solución `.dll` asociada.

## Imágenes & tipografía

Los iconos e imágenes se incluirán de forma manual a través de gestor de contenidos DNN. Preferiblemente en formato .svg y .webp.
Ante la imposibilidad de incluir la tipografía **Montserrat** de **Google Fonts** a través del DNN se ha incluido en el código CSS a través de la etiqueta `@import`.

## Arquitectura

Según los requisitos del proyecto únicamente se cambiará la capa de presentación de la web por lo que no se tocará nada de la estructura original salvo pequeñas modificaciones del contenido para adaptar la maquetación al prototipo.

## Metodología

Se mantendrá la metodología original para que el resto de capas de la aplicación no se vean afectadas.
En caso de necesitar modificar algún componente se usará la metodología BEM (*se detalla en la guía de estilos*) para el nombrado de clases de la hoja de estilo.

