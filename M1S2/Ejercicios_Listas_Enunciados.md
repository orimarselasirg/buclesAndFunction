# 🧩 Ejercicios de Listas en Python (Funciones + Validaciones/Bucles)

Todos los ejercicios deben:
- Implementar **al menos una función**.
- Usar **validaciones** y/o **bucles**.
- Manipular listas con **métodos de listas**.

**1) Restaurante “Menú Dinámico” — Agregar plato del día**  
*Como chef,* quiero una función `agregar_plato(menu, plato)` que **valide** que `plato` no esté vacío y **lo agregue** a la lista `menu`.  
- Si el plato ya existe, mostrar “plato duplicado”.  
- Recorre el menú al final para imprimirlo numerado.  
**Sugerencia:** usa `list.append()`.

**2) Teatro “Butacas VIP” — Insertar reserva en posición**  
*Como encargado de reservas,* quiero una función `insertar_reserva(butacas, nombre, posicion)` que **valide** que `posicion` esté en rango y **ubique** la reserva en esa posición.  
- Si la posición no es válida, no inserta y muestra error.  
- Luego, recorre la lista para confirmar el orden.  
**Sugerencia:** usa `list.insert()`.

**3) Tienda “Combo Pack” — Extender inventario**  
*Como supervisor,* quiero una función `extender_inventario(actual, nuevos)` que **valide** que `nuevos` no esté vacío y **una** ambas listas.  
- Muestra el tamaño total al final.  
- Recorre la lista para destacar los recién agregados.  
**Sugerencia:** usa `list.extend()`.

**4) Biblioteca “Depuración de catálogo” — Eliminar libro específico**  
*Como bibliotecario,* quiero una función `eliminar_libro(catalogo, titulo)` que **verifique** si el título está y **lo quite**.  
- Si no existe, mostrar “no encontrado”.  
- Imprimir los libros restantes con un bucle.  
**Sugerencia:** usa `list.remove()`.

**5) Cine “Liberar última silla” — Quitar el final**  
*Como administrador de sala,* quiero una función `liberar_ultima(butacas)` que **valide** que hay elementos y **quite** el último asiento reservado; debe **retornar** el valor removido.  
- Si no hay butacas, mostrar “sala vacía”.  
- Imprimir el estado final.  
**Sugerencia:** usa `list.pop()` sin índice.

**6) Soporte “Búsqueda de ticket” — Encontrar primera coincidencia**  
*Como agente de soporte,* quiero una función `buscar_ticket(tickets, codigo)` que **valide** si `codigo` está y devuelva su **índice**.  
- Si no existe, retorna `-1`.  
- Usa un bucle para confirmar si hay duplicados y contarlos.  
**Sugerencia:** usa `list.index()` (maneja excepciones) y/o `list.count()`.

**7) Deportes “Marcador frecuente” — Contar apariciones**  
*Como estadístico,* quiero una función `contar_marcador(marcadores, valor)` que **valide** tipos y devuelva cuántas veces aparece `valor`.  
- Si no aparece, retornar 0.  
- Recorre la lista para imprimir posiciones donde aparece.  
**Sugerencia:** usa `list.count()`.

**8) Academia “Registro ordenado” — Orden asc/desc configurable**  
*Como coordinador,* quiero una función `ordenar_registros(registros, descendente=False)` que **valide** que todos los elementos sean comparables y ordene.  
- Si `descendente` es `True`, ordenar en orden inverso.  
- Recorre la lista para imprimir el TOP 3.

**9) Música “Playlist Reversa” — Escucha en orden invertido**  
*Como DJ,* quiero una función `invertir_playlist(playlist)` que **valide** que no esté vacía y **la invierta en sitio**.  
- Luego, recorre la lista para reproducir las primeras 5 canciones (o menos si no hay suficientes).

**10) Cursos “Duplicar plan de estudio” — Copia segura**  
*Como tutor,* quiero una función `clonar_plan(modulos)` que **cree una copia** independiente de la lista original para probar cambios sin afectar la original.  
- Verifica con un cambio en la copia que la original no se altere.  
- Usa bucles para mostrar diferencias.

**11) Logística “Limpieza de ruta” — Vaciar lista al finalizar**  
*Como coordinador de ruta,* quiero una función `finalizar_ruta(paradas)` que, tras recorrer y marcar cada parada como “visitada”, **limpie** la lista.  
- Valida si ya está vacía antes de limpiar.  
- Muestra un mensaje final de confirmación.

**12) Aula “Control de asistencia” — Sustitución por índice**  
*Como docente,* quiero una función `marcar_asistencia(estudiantes, indice, estado)` que **valide** el índice y reemplace el valor en esa posición por `estado`.  
- Si el índice es inválido, no modifica la lista.  
- Recorre para contar presentes/ausentes.

**13) E-commerce “Carrito flexible” — Agregar/Quitar según acción**  
*Como comprador,* quiero una función `actualizar_carrito(carrito, accion, item, posicion=None)` que:  
- Si `accion` es “agregar”, agregue `item` al final o en `posicion` válida.  
- Si `accion` es “quitar”, retire por nombre o por índice (si `posicion` es un entero).  
- Valida entradas y usa bucles para mostrar el total de items.

**14) RRHH “Top talentos” — Mezclar y ordenar candidatos**  
*Como reclutador,* quiero una función `fusionar_candidatos(base_a, base_b, clave_desc=False)` que **combine** dos listas y **ordene** asc/desc según `clave_desc`.  
- Valida que ambas listas contengan el mismo tipo de dato.  
- Recorre para imprimir los primeros N candidatos.

**15) Ventas “Depurar duplicados” — Primero elimina, luego compacta**  
*Como analista,* quiero una función `depurar_ventas(ventas, umbral)` que:  
- Recorra la lista y **elimine** valores no válidos (negativos o `None`).  
- Si un valor se repite más de `umbral`, **retira** las apariciones extra hasta dejar `umbral`.  
- Muestra la lista final y la cantidad de elementos removidos.
