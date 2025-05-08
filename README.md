# Ejemplo HTML + Bootstrap 🖥️

Este ejemplo consta de 4 archivos:

1. `Readme.md`, en donde se encuentra la consigna.
2. `Index.html`, en donde se encuentra un archivo con la estructura básica de un html sobre el cuál se podrá trabajar sobre la consigna.
3. `solucion.html`, con una posible solución.
4. `boostrap_gallery_app.html`, un archivo con ejemplos de componentes de Boostrap (independiente de este ejemplo)

## Requerimientos previos:
**1.** Instalar la extensión **Live Preview** para visualizar en tiempo real los cambios realizados en el código HTML directamente en el navegador.
 
## Pasos:

### 1. Configuración Bootstrap:
Bootstrap es un framework de CSS que permite crear diseños modernos y responsivos rápidamente sin escribir mucho código.

**1.** Para enlazar el archivo CSS de Bootstrap, sin necesidad de instalar nada, copiar y pegar el siguiente fragmento de código en el head de nuestro `index.html`. Si hay otras hojas de estilo, se debera hacer previo a la declaración de estas:

``` 
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous"> 
```
**2.** Para habilitar componentes interactivos (botones, menús desplegables, etc.), copia el siguiente bloque de código antes de cerrar el `</body>` en nuestro `index.html`
```
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>
```

Opcional: Si se desea habilitar íconos, debajo de dónde se agregó la linea de código en el paso 1, agregar:
```
<link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.5/font/bootstrap-icons.css" rel="stylesheet">
```

### 2. HTML:

**1.** Crear un formulario básico en HTML.
Incluir los siguientes campos:
- Nombre (input de texto)
- Correo electrónico (input de tipo email)
- Mensaje (textarea)
- Botón de envío
  
```
<h1>Formulario de Contacto</h1>

<form>
  <label for="nombre">Nombre:</label><br>
  <input type="text" id="nombre" name="nombre"><br><br>

  <label for="email">Correo electrónico:</label><br>
  <input id="email" name="email"><br><br>

  <label for="mensaje">Mensaje:</label><br>
  <textarea id="mensaje" name="mensaje"></textarea><br><br>

  <button type="submit">Enviar</button>
</form>
```

2. Manejo de errores (Desde HTML):
- Validar que el campo de mail tenga formato de mail (pista: type)
- Validar que se ingresó el nombre y el mail al momento de enviar el formulario (pista: requiered).

### 3. Boostrap:
> 💡 Los siguientes pasos deben ser realizados utilizando componentes de Boostrap.

**Containers:**

**1.** Agregar un [Container](https://getbootstrap.com/docs/5.0/layout/containers/) que envuelva al formulario. 

**Espaciados:**

**2.** Agregar [espaciado](https://getbootstrap.com/docs/5.0/utilities/spacing/) entre el título y el formulario
    *Sugerencia*: Agregar las clases de margin, como por ejemplo mt-5 y mb-4 al título del formulario
    
**Formularios:**

**3.** Agregar la clase form-label y la clase form-control a las labels y los inputs del formulario. Agregar la clase form-group. [Formularios](https://getbootstrap.com/docs/4.0/components/forms/)

**4.** Reemplazar las etiquetas `<br>` por spacings donde sea necesario. Ajustar espaciados con las clases mt y mb.

**5.** Agregar dos RadioButtons (botones de opción) para que el usuario pueda seleccionar si es alumno o docente. [Radios y checkboxes](https://getbootstrap.com/docs/5.0/forms/checks-radios/)

**6.** Agregar un checkbox para verificar si el usuario acepta los términos y condiciones. [Radios y checkboxes](https://getbootstrap.com/docs/5.0/forms/checks-radios/)

Opcional:
- Cambiar los inputs a alguna de las siguientes opciones:
- 
[Input group](https://getbootstrap.com/docs/4.0/components/input-group/)

[Floating labels](https://getbootstrap.com/docs/5.0/forms/floating-labels/)

 
**Botones:**

**7.** Cambiar el botón provisto en el HTML por un [botón](https://getbootstrap.com/docs/4.0/components/buttons/) de tipo **primario**.

**8.** Agregar un botón secundario que presente la opción de Cancelar.

**9.** Seleccionar un ícono de la [librería de íconos de Boostrap](https://icons.getbootstrap.com/icons/) y agregarselo al botón de enviar.
**IMPORTANTE:** Es necesario haber agregado la configuración para íconos previamente (revisar paso 1).


**Card:**

**10.** Envolver el formulario en una [Card](https://getbootstrap.com/docs/5.3/components/card/) y ajustar el padding y los márgenes a gusto.

**Colores**
- Cambiar el color de los componentes a través de un archivo `styles.css`. 
  
**Responsive y accesibilidad:**
- Comprobar que el sitio obtenido es Responsive.
- **Extra:** Comprobar con la herramienta WAVE que no hayan errores o warnings de accesibilidad.
  
> En el archivo `solucion.html` se encuentra una posible solución a este ejemplo

## Recursos:

- [Repaso HTML](https://www.w3schools.com/html/html_intro.asp)
 
- [Documentación Boostrap](https://getbootstrap.com/docs/5.0/getting-started/introduction/)
