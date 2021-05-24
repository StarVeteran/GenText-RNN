# GenText-RNN
Una red neuronal recurrente simple para generar textos.

Apartir de una lista de palabras en un archivo de texto, genera texto aleatorio en base a los caracteres de la lista que se proporciona.

Este modelo usa una RNN simple y no LSTM. Las entradas de este modelo son los caracteres, luego se usa un vector como entrada. La dimension de X es del tamaño de los caracteres de la entrada del archivo.

Este modelo RNN simple tiene 3 matrices:

---- Whh: H*H , capa oculta a capa oculta

---- Wxh: V*H, capa de entrada a capa oculta

---- Why: V*H, capa oculta a capa de salida

En la capa de salida, la funcion softmax es usada para calcular la propabilidad de distribucion, luego se muestrea el siguiente caracter de acuerdo a la entrada previa.
