# asmjs-fibonacci
Hola mundo de ASM.JS compilado con CHEERP desde C++, fibonacci de 45 para probar diferencia de rendimiento.

En C++ exportamos la funcion fib exportando el objeto ModulosExportados usando la notacion-namespace [[cheerp::jsexport]].
Asi se puede llamar desde el javascript normal del html a nuestra funcion fib implementada en C++ y compilada a ASM.JS
El acceso desde el javascript normal al objeto exportado es directo y el uso de fib es publico: 
var modExporASM = new ModulosExportados();
var resultado = modExporASM.fib(45);
