# Gestion de Datos

This project consists in a JS code that I used to practice Arrays, set, map, for in, for of, and forEach.


## Table of Contents
- gestion_datos
- Technologies Used
- How To Use


## gestion_datos

This is the JS code where I put the code to practice.


## Technologies Used

- Visual Studio
- JavaScript
- Google Chrome


## How to use

1. Copy the next code.
2. Open a navigator.
3. Right Click and Inspection.
4. Click in the console.
5. Paste the code and press Intro.


  ```bash
       /* I create an object */
    const productos = {
        1: {id: 1, nombre: "PC", precio: 4000000},
        2: {id: 2, nombre: "Auriculares", precio: 300000},
        3: {id: 3, nombre: "Teclado", precio: 50000}
    };
    console.log("Este es el objeto llamado 'productos'",productos);
    
    /* I create a set using the values of productos object */
    const setProductos = new Set(Object.values(productos).map(producto => producto.nombre));
    console.log("Set de produtos unicos:", setProductos);
    
    /* I create a map*/
    const mapProductos = new Map([
        ["Electrodomestico", ["PC"]],
        ["Accesorio", ["Auriculares", "Teclado"]]
    ]);
    console.log("map de productos", mapProductos);
    
    /* Here I iterate products by id and their specifications */
    for (const id in productos) {
        console.log(`Producto ID: ${id}, Detalles:`, productos[id]);
    };
    
    /* Here I iterate products of setProductos */
    for (const producto of setProductos) {
        console.log("Producto:", producto);
    };
    
    /* Here with forEach I iterate mapProductos */
    mapProductos.forEach((producto, categoria) => {
        console.log(`Categoria: ${categoria}, Producto: ${producto}`);
    });
    
    /* Results */
    console.log("Lista de productos:", productos);
    console.log("Lista de productos unicos:", setProductos);
    console.log("Categoria de productos:", mapProductos);

   ```
