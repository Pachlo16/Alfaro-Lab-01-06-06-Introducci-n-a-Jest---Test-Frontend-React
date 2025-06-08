# Escenarios de la Historia de Usuario: Gestionar cupones en la vista de admin

## Historia de Usuario
Como administrador quiero poder crear, activar/desactivar y eliminar cupones de descuento, para gestionar las promociones disponibles en la plataforma.



### Happy Paths

#### 1. Crear un cupón válido
- El admin ingresa un código, una descripción y un porcentaje de descuento válido (por ejemplo, 15).
- Presiona "Añadir".
- El cupón aparece en la lista de cupones activos.

#### 2. Activar/Desactivar un cupón
- El admin visualiza la lista de cupones.
- Presiona el botón "Desactivar" en un cupón activo.
- El estado del cupón cambia a "Inactivo".
- Presiona el botón "Activar" en un cupón inactivo.
- El estado del cupón cambia a "Activo".

#### 3. Eliminar un cupón
- El admin visualiza la lista de cupones.
- Presiona el botón "Eliminar" en un cupón.
- El cupón desaparece de la lista.



### Unhappy Paths

#### 1. Intentar crear un cupón con campos vacíos
- El admin deja uno o más campos vacíos (código, descripción o descuento).
- Presiona "Añadir".
- El cupón no se agrega y los campos permanecen igual.

#### 2. Ingresar un porcentaje de descuento inválido
- El admin ingresa un valor no numérico o un número menor o igual a 0 o mayor a 100 en el campo de descuento.
- Presiona "Añadir".
- El cupón no se agrega y los campos permanecen igual.

#### 3. Eliminar un cupón inexistente
- El admin intenta eliminar un cupón que ya no está en la lista (por ejemplo, por un error de sincronización).
- El sistema ignora la acción y la lista permanece sin cambios.

# Alfaro-Lab-01-06-06-Introducci-n-a-Jest---Test-Frontend-React
