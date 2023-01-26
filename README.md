## **Lista Ligada Simple**

El proyecto contiene las siguientes clases:

* **`LinkedList`** donde se establece la lógica de la lista ligada simple
* **`Node`** contiene la informacion de un nodo
* **`test`** prueba un ejemplo para observar el funcionamiento de la lista ligada simple

### **Tipo de Lista**

A continuación describimos las caracteristicas de una Lista Ligada Simple.

**Lista Simple** En la siguiente imagen podemos ver cómo se enlazan los nodos con el Nodo siguiente (Pueden tener un enlace o dos enlaces dependiendo del tipo de Nodo). En una lista simple el ultimo nodo de la lista siempre apunta a **null**

![Simple](https://user-images.githubusercontent.com/115047831/207787125-de59c66c-3e98-4ad2-a570-4f4c5ceb69ba.png)

### **Tipo de Nodo**

**Nodo Simple** Un Nodo simple tiene un único apuntador y siempre apuntará al siguiente Nodo.

![Unique](https://user-images.githubusercontent.com/115047831/207787501-3af9c726-4cce-4120-8b49-2bac880bd026.png)

## Agregar Nodo

**Cuando agregamos un nuevo Nodo siempre se añadira al final de la Lista**

Tenemos la siguiente lista con los siguientes nodos: Nodo 2 (Rojo) y Nodo 3 (Amarillo), si queremos agregar el Nodo 4 (Verde) entonces el apuntador del Nodo 3 (Amarillo) ahora debera apuntar al Nodo 4 (Verde).

![SimpleLinkedList5](https://user-images.githubusercontent.com/115047831/214767401-f851156c-3cb0-4471-8bcb-e4a2eb8ba757.png)

Ahora que agregamos el Nodo 4 (Verde) debemos saber que la **variable last** esta apuntando al Nodo 4 (Verde) ya que ahora es el último nodo de la lista.

![SimpleLinkedList6](https://user-images.githubusercontent.com/115047831/214767485-c7143d19-aa8e-4c35-9637-d645080502c0.png)

## Eliminar Nodo

**Se elimina un Nodo por su valor númerico, se elimnarán todos los valores con este dígito.**

En el siguiente ejemplo podemos observar que el Nodo 1 (Azul) se repite 5 veces en la lista, el objetivo es eliminar todos los nodos que coinciden con el número 5, independientemente de su posición en la lista deberán ser eliminados. El método **`delete`** se compone de tres partes, si identifica que el Nodo ha eliminar está al inicio de la lista  entonces ejecutará el método **`deleteFirst`** mientras que detecte que el valor sigue al inicio de la lista. Posteriormente buscará el nodo que esta al final de la lista, si coincide con el número a eliminar continuara eliminandolo ejecutando el método **`deleteLast`** hasta que no este al final de la lista. Finalmente buscará el valor númerico del nodo unicamente en el medio de la lista.

![SimpleLinkedList7](https://user-images.githubusercontent.com/115047831/214769720-e9d21bfe-60a3-4619-b660-0c620d9bbc7f.png)

En la siguiente imagen podemos observar que todos los Nodos 1 (Azul) han sido removidos de la lista.

![SimpleLinkedList8](https://user-images.githubusercontent.com/115047831/214769768-95a31296-bdca-477c-92fc-f6581c04606a.png)

## Diagrama de clases con UML

> **Nota:** El siguiente diagrama de clases representa la lógica de programación utilizada para construir la **Lista Ligada Simple**. La clase **test** no se incluye en el diagrama UML porque solo contiene el método main y únicamente es utilizada para demostrar el funcionamiento de los métodos de la lista.

![UML](https://user-images.githubusercontent.com/115047831/214760358-215cbaaa-bd41-4e52-b94d-1c131f46d437.png)
