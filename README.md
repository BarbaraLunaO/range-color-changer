## Input Range con Cambio de Color Dinámico

https://raw.githubusercontent.com/BarbaraLunaO/range-color-changer/blob/main/ranges-colors.png

Este proyecto es un ejemplo de cómo crear un input range en HTML que cambia de color en tiempo real según el valor 
seleccionado. Utiliza CSS para estilizar el rango y JavaScript para controlar el cambio de color dinámico. Además, 
Flask se utiliza como servidor web para visualizar el resultado en el navegador.


## Requisitos
- Crear tu entorno virtual y descargar Flask

##Instrucciones de uso
Elegir los cuatro colores de estado para el range o usar los actuales (amarillo-naranja-rojo-marron)
```javascript
if (value >= 0 && value <= 2) {
        color = "yellow";
      } else if (value >= 3 && value <= 5) {
        color = "orange";
      } else if (value >= 6 && value <= 8) {
        color = "red";
      } else if (value >= 9 && value <= 10) {
        color = "brown";
      }
```
Los range values van de 0-10 de 1 en 1, en caso de cabiar el valor max recuerda
cambiar el valor multiplicativo para calcular el gradiente en el css
``` css
background-image:linear-gradient(to right, var(--color)  calc(var(--value)*10%), white 0);
```

##Contribuciones
Las contribuciones son bienvenidas. Si encuentras algún problema o tienes una mejora, no dudes en abrir un problema o enviar una solicitud de extracción.

##Licencia
Este proyecto está bajo la Licencia MIT.





