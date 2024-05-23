# Examen - Nutrientes saludables

## Enunciado 
Una vez se ha puesto en marcha la primera versión de Deliver US, los inversores han solicitado la inclusión de una nueva funcionalidad que consiste en informar al cliente de los gramos de macronutrientes que contienen cada uno de los productos. Tras la reunión con el cliente, se ha establecido los siguientes requisitos:

1.- Debido a la normativa reguladora de alimentación, se pide que se informe al cliente de la cantidad de carbohidratos, proteínas y grasas por cada 100 gramos de cada uno de los productos que están a la venta en Deliver US.

2.- Dada la existencia de platos hipercalóricos que no están recomendados en una dieta saludable se pide que un plato no pueda contener más de 1000 calorías por 100g de producto. Para ello, se usará la siguiente formula aproximada de cálculo energético
Calorías producto = (grasas *9) + (proteínas * 4)+(carbohidratos * 4)

Se pide que:

1.- Implemente los cambios que sean necesarios en el backend.

2.- Implemente validación de servidor y cliente con los requisitos de calorías máximas.

3.- Muestre los datos de calorías por 100g, carbohidratos, proteínas y grasas en cada uno de los productos que se muestran en la pantalla RestaurantDetailScreen.

Nota: No es necesario modificar los seeders. Recuerde que los valores numéricos enviados por el frontend, llegan al backend como string cuando se usan TextInputs en el componente InputItem. No olvide realizar un casting a float de dichos valores para que el backend los trate sin problema.

## Introducción

Este repositorio incluye el backend completo (carpeta `DeliverUS-Backend`) y el frontend de `owner` (carpeta `DeliverUS-Frontend-Owner`). Servirá como base para realizar el examen de laboratorio de la asignatura.

## Preparación del entorno

### a) Windows

* Abra un terminal y ejecute el comando `npm run install:all:win`.

### b) Linux/MacOS

* Abra un terminal y ejecute el comando `npm run install:all:bash`.

## Ejecución

### Backend

* Para **rehacer las migraciones y seeders**, abra un terminal y ejecute el comando

    ```Bash
    npm run migrate:backend
    ```

* Para **ejecutarlo**, abra un terminal y ejecute el comando

    ```Bash
    npm run start:backend
    ```

### Frontend

* Para **ejecutar la aplicación frontend de `owner`**, abra un nuevo terminal y ejecute el comando

    ```Bash
    npm run start:frontend:owner
    ```

## Depuración

* Para **depurar el backend**, asegúrese de que **NO** existe una instancia en ejecución, pulse en el botón `Run and Debug` de la barra lateral, seleccione `Debug Backend` en la lista desplegable, y pulse el botón de *Play*.

* Para **depurar el frontend**, asegúrese de que **EXISTE** una instancia en ejecución del frontend que desee depurar, pulse en el botón `Run and Debug` de la barra lateral, seleccione `Debug Frontend` en la lista desplegable, y pulse el botón de *Play*.

## Test

* Para comprobar el correcto funcionamiento de backend puede ejecutar el conjunto de tests incluido a tal efecto. Para ello ejecute el siguiente comando:

    ```Bash
    npm run test:backend
    ```
**Advertencia: Los tests no pueden ser modificados.**
