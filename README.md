# MAtlab
Course of Matlab

### variable a  

#### commands

*whos a*   
 Name     Size     Bytes    Class    Attributes  
 
 *Memory*  
 
 a=single(pi) --> 4bytes  
 a=int8(pi) --> 8bytes  
 a=int64(pi) -->64bytes  
 
 ## Matrix  
  A=[fila1 ; fila2; ...]  
  A=[fila1; ...   
     fila2;...
     filan]  
*Strings*  
a='hola'  

## Excel  
matrices de celdas  
archivo guardado como 'prueba.xls'

[num , txt, raw ]= xlsread('Prueba.xls')
raw lo lee todo y devuelve una matriz de matrices    

info(1 linea).nombre=raw[1,1]   (posición)  
info(1).nota=raw[1,2]  
info(1).fecha=raw[1,3]  

info(2).nombre.....  

Por ejemplo  
info(1)   
nombre:  Juan  
fecha:  1/4/99  
nota: 3  

LLAMADA DE UNA FUNCION EN MATLAB  
[variables de salida]=Fun(variables de entrada)  

## Operaciones con matrices  





