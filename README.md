![mayusculas javascript](https://raw.githubusercontent.com/sergiecode/get-modifier-state-js/master/getModifierState.jpg)


# Tutorial de Aviso al Usuario sobre el Uso de Mayúsculas

Este repositorio contiene un pequeño código JavaScript que te permite notificar a los usuarios cuando la tecla "Caps Lock" está activada. El propósito de esta funcionalidad es proporcionar a los usuarios una indicación visual de si tienen activada la tecla de mayúsculas, lo que puede evitar errores al ingresar contraseñas u otros datos sensibles en formularios.

## Instrucciones de Uso

Sigue estos pasos para incorporar la funcionalidad de aviso al usuario sobre el uso de mayúsculas en tu proyecto:

1.  **Incorporar el Código JavaScript**
    
    Agrega el siguiente fragmento de código JavaScript en tu archivo HTML, generalmente dentro de la etiqueta `<script>` o en un archivo externo `.js` vinculado:
    
    ```
    
    document.addEventListener('keydown', function(event) {
        if (event.getModifierState('CapsLock')) {
            // La tecla CapsLock está activada
            // Aquí puedes agregar el código para mostrar una notificación o cambiar el estilo visual
            // para indicar que la tecla CapsLock está activada.
        } else {
            // La tecla CapsLock está desactivada
            // Aquí puedes agregar el código para ocultar la notificación o restablecer el estilo visual.
        }
    });
    ```
    
2.  **Personaliza las Acciones**
    
    En los comentarios dentro del código, encontrarás los lugares donde puedes agregar tu propio código para mostrar o ocultar notificaciones visuales. Esto podría incluir mostrar un mensaje en pantalla, cambiar el color de fondo de un elemento o cualquier otra acción visual que consideres apropiada para indicar el estado de "Caps Lock".
    
3.  **Adapta el Diseño**
    
    El código proporcionado se enfoca en la lógica funcional y no aborda el diseño visual específico. Asegúrate de personalizar el diseño y la experiencia de usuario de acuerdo con el estilo de tu proyecto.
