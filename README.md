# SweetAlert Tutorial 🚀

Este repositorio contiene un tutorial sobre **SweetAlert**, una librería para mostrar alertas personalizadas en JavaScript. Aprende a mejorar la experiencia de usuario con mensajes interactivos y atractivos.

## 📌 Instalación

SweetAlert se puede instalar de varias formas:

### 🔹 Usando CDN (recomendado para pruebas rápidas)
```html
<script src="https://cdn.jsdelivr.net/npm/sweetalert2@11"></script>
```

### 🔹 Usando npm (para proyectos más grandes)
```sh
npm install sweetalert2
```

## 🚀 Uso Básico

Ejemplo de una alerta simple:
```js
Swal.fire('¡Hola!', 'Esta es una alerta básica con SweetAlert.', 'success');
```

## 🎨 Personalización de Alertas

### 🔹 Agregar un botón de confirmación
```js
Swal.fire({
  title: '¿Estás seguro?',
  text: 'No podrás revertir esto.',
  icon: 'warning',
  showCancelButton: true,
  confirmButtonText: 'Sí, eliminar',
  cancelButtonText: 'Cancelar'
});
```

### 🔹 Agregar un input en la alerta
```js
Swal.fire({
  title: 'Ingrese su nombre',
  input: 'text',
  showCancelButton: true,
  confirmButtonText: 'Guardar'
}).then((result) => {
  if (result.isConfirmed) {
    Swal.fire(`Nombre guardado: ${result.value}`);
  }
});
```

## 📽️ Ejemplos en Video

Consulta el video en YouTube donde mostramos estos ejemplos en acción: **[Enlace aquí]**

## 🤝 Contribuciones
Si quieres agregar más ejemplos o mejorar el tutorial, ¡las contribuciones son bienvenidas! 😊

## 📜 Licencia
Este proyecto se distribuye bajo la licencia MIT.
