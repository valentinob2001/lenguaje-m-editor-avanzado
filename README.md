# lenguaje-m-editor-avanzado
Práctica M6 S8

Dado el caso de que hubiera utilizado Text.Upper en vez de Text.Proper para estandarizar la categoria, en el filtro de los registros de prueba debería especificar que se busca el valor "PRUEBA" y no "Prueba". Esto se debe a que la función Text.Upper convierte en mayúscula todos los caracteres del texto en cuestión.

Como en este script la función Text.Trim se aplica únicamente a la columna "nombre_producto", los registros con la categoría "prueba " no serían eliminados. Para lograr que eso suceda no es necesario agregar un paso, es suficiente con agregar una lista anidada en el paso 2 del tipo {{"categoria", Text.Trim, type text}}, en tanto ya estamos definiendo una función que se llama LimpiarEspacios.

En relación a la diferencia entre Text.Trim y Text.Clean yace en que mientras la primera función elimina únicamente espacios al principio y al final, la segunda elimina además caracteres ocultos.

Con respecto a la última pregunta, entiendo que estandarice los registros de la categoría antes de filtrar debido a que de lo contrario no se hubieran estandarizado los registros con la palabra "PRUEBA" por no estar presentes en el resultado anterior.
