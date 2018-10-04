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
 
xlswite('Plantilla.xls',Nodos,'Nodos','B2')    
xlsread('Plantilla.xls','Nodos')  
hoja de cálculo Plantilla pestaña Nodos


LLAMADA DE UNA FUNCION EN MATLAB  
[variables de salida]=Fun(variables de entrada)  
function  
[y1,y2]=nombredelaFuncion(x)  

## Operaciones con matrices  

logaritmo neperiano log(x)   
logaritmo en base 10 log10(x)  
sin(vector) = seno de cada elemento del vector de la matriz  
x=[ -2:0,1:2] desde menos 2 hasta 2 cada 0.1  
elevar al cubo elementos de una matriz x.^3
plot(x,y)  
grid on --- grid off regilla  
xlabel ('Ejex')
ylabel('Eje y')
axis([-1 1 -0.1 2.2])
axis([ejex ejey])  
sort --> ordena vectores o tablas  
find(A(:,1)==1)--> matriz A en todas las filas en la primera columna cual tiene valor igual a 1  



D=[A C ;B] 
MAtriz A y C se suman en horizontal    
MAtriz AC se suma a B en vertical  

*Diagonales*  
diag([1 2 3 4] ) 
diag([1 2 3 4] , -1) la mueve hacia abajo  
diag([1 2 3 4] , 2) la mueve hacia arriba  
la inversa de una matriz ecuación D * x= b --> b vector columna   
x = D\b
Transpuesta A'  
inversa pinv(A)


[X,Y]=meshgrid(x,y);
convierte vectores en matrices cuadradas

*Dibujo 3D*  
surf(x,y,z)  
shading interp  elimina rallas y da mas color  
shading faceted  
colormap copper 
plot(x,y)  
hold on --> para dibujar otra  
legend('lenyenda1','leyenda2')  
title('titulo')  
close --> cerrar dibujo  
figure(1);
imagesc(A)--> colores por números de la matriz  





**Bucle**  
y=NaN(1,4); for i=i:4, y(i)=sin(x(i)), end
y=NaN(1,4); for i=i:length(x), y(i)=sin(x(i)), end


**Rutina**
function [y,dy]=Mifunction(x)  

    y =2*x.^2+x+3;  
end  

Fichero principal  
[y,dy]= Mifunction(3)
  return  -->  y= 24 dy=13  
  
if nargin<2 --> si el número de argumentos de entrada es menor que dos  


** BARRAS**  

 Nodos y Barras  
 Nodos con cordenadas en el plano (x,y)  
 
 Nodos  
 (x1,y1) primer  
 (x2,y2) segundo  
 (x3,y3) tercero  
 
 Barras --> Matriz barras (Matriz de conectividad)  
 
           *Nodos*  
 Barra  1------    1 ---      2  
 Barra  2------    2 ---      3  
 
   VAlor mas grande de una matriz  
 kmax=max(abs(K(:)))  
máxima relacion para que el valor sea máximo es 1e16  
el límite total seria k_inf=1e16  

  
  







