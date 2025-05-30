El proyecto trata sobre un pequeño sistema de gestión de una concesionaria de vehículos (autos y motos) en Java, utilizando Programación Orientada a Objetos. 
Permite almacenar vehículos con sus atributos (marca, modelo, precio, etc.), filtrar y ordenarlos a partir de diferentes criterios y mostrar información por consola.

El proyecto está creado con Spring Boot, gestionado con Maven y utiliza Lombok para evitar el "boilerplate" (codigo repetitivo).

Caracteristicas principales:
La clase abstracta Vehiculo sirve como base para las clases Auto y Moto, permite representar las propiedades de cada tipo de vehículo. Cada clase sobreescribe su propia versión del método .toString() para mostrar la información de manera clara, incluyendo el precio con el formato adecuado.
El sistema funcionalidades de ordenamiento, como organizar los vehículos por precio de mayor a menor o seguir un orden natural basado en la marca, modelo y precio. Además, incluye operaciones de búsqueda específicas, tales como buscar el  vehículo más caro o más barato, y filtrar los que en el modelo contengan una letra específica.
Se utiliza DecimalFormat en todos los precios, mostrándolos con separadores de miles y decimales (según el formato de la región). Esto asegura que la información sea fácil de leer.

Ejecución:
La ejecución del programa se hace en la clase TestsConcesionaria. Al iniciarse, el sistema carga automáticamente los vehículos y muestra (en el orden que se ingresaron) la lista de autos y motos disponibles en la consola.
Paso seguido, el programa muestra los resultados de las operaciones: vehículo más caro y más barato, los modelos que contienen una letra específica en su modelo, y las listas ordenadas por precio (de mayor a menor) y por orden natural.
