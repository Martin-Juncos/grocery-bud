# Proyecto Grocery Bud en JavaScript

### Descripción del Proyecto

El proyecto Grocery Bud es una aplicación web simple para la gestión de una lista de compras, desarrollada utilizando JavaScript, HTML y CSS. Esta aplicación permite a los usuarios agregar, editar y eliminar elementos de su lista de compras, ofreciendo una experiencia de usuario interactiva y amigable.

### Propósito del Proyecto

El propósito de este proyecto es proporcionar una herramienta útil para organizar y gestionar las compras del supermercado de manera eficiente. La aplicación está diseñada para ser fácil de usar y ofrece funcionalidades básicas que pueden ser expandidas según las necesidades del usuario.

### Lógica del Código

El proyecto utiliza JavaScript para manejar la interacción del usuario y actualizar la interfaz de usuario en tiempo real. A continuación, se describe la lógica principal del código:

1. **Estructura HTML**:
   La estructura HTML define los elementos básicos de la aplicación, incluyendo un campo de entrada para los nuevos ítems, un botón para agregar ítems y una lista para mostrar los ítems agregados.

   ```html
   <div class="grocery-form">
     <input type="text" id="grocery-input" placeholder="e.g. eggs" />
     <button id="grocery-submit">Submit</button>
   </div>
   <div class="grocery-container">
     <ul id="grocery-list"></ul>
   </div>
   ```

2. **Agregar Ítems**:
   Al hacer clic en el botón "Submit", el valor del campo de entrada se agrega a la lista de compras y se muestra en la interfaz de usuario. Si el campo está vacío, se muestra un mensaje de error.

   ```javascript
   document.getElementById("grocery-submit").addEventListener("click", addItem);

   function addItem() {
     const input = document.getElementById("grocery-input");
     const value = input.value.trim();
     if (value) {
       // agregar ítem a la lista
     } else {
       // mostrar mensaje de error
     }
   }
   ```

3. **Editar y Eliminar Ítems**:
   Cada ítem de la lista tiene botones para editar y eliminar. Al hacer clic en el botón de editar, el ítem se carga en el campo de entrada para su modificación. Al hacer clic en el botón de eliminar, el ítem se elimina de la lista.

   ```javascript
   function editItem(id) {
     // cargar ítem en el campo de entrada para editar
   }

   function deleteItem(id) {
     // eliminar ítem de la lista
   }
   ```

4. **Persistencia de Datos**:
   La lista de compras se guarda en el almacenamiento local del navegador para que los datos persistan incluso después de recargar la página.
   ```javascript
   localStorage.setItem("groceryList", JSON.stringify(groceryList));
   ```

### Uso de la Aplicación Grocery Bud

1. **Abrir el Archivo**:
   Abre el archivo `index.html` en tu navegador para ver la aplicación en acción.

2. **Agregar Ítems**:
   Escribe el nombre del ítem que deseas agregar en el campo de entrada y haz clic en el botón "Submit". El ítem aparecerá en la lista de compras.

3. **Editar Ítems**:
   Para editar un ítem, haz clic en el botón de editar (ícono de lápiz) junto al ítem. El ítem se cargará en el campo de entrada para que puedas modificarlo. Luego, haz clic en "Submit" para guardar los cambios.

4. **Eliminar Ítems**:
   Para eliminar un ítem, haz clic en el botón de eliminar (ícono de basura) junto al ítem. El ítem se eliminará de la lista.

### Modificación de la Aplicación

Para modificar el comportamiento de la aplicación Grocery Bud, puedes cambiar el código JavaScript. También puedes modificar el CSS y el HTML para cambiar la apariencia de la página y de los ítems de la lista.

                     ©ProfMartinJuncos2024

```

```
