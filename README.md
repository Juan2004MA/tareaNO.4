# tarea4Algortitmo
## Ejercicio 1: 
escriba una aplicación para resolver el siguiente enunciado. El gobierno ha implementado
como parte de su programa social, un subsidio familiar bajo la siguiente reglamentación:
Las familias que tienen hasta 2 hijos, reciben Q. 70.00, las que tienen hasta 3 y 5 reciben Q. 90.00 y las
que tienen 6 o más reciben Q. 120 mensual. Por cada hijo en edad escolar reciben Q. 10.00 adicionales.
Se considera la edad escolar entre 6 y 18 años. Si la madre de familia fuera viuda, la familia recibe Q.
20.00 adicionales.
Determinar el monto mensual que recibirá una familia de acuerdo a su realidad familiar a través de una
función llamada calcularSubsidio

##codigoNO1.
```C++
//calcular subsidio de las mamás

#include <iostream>
using namespace std;

int main {
def calcularSubsidio (num_hijos, edades_escolares,es_viuda):

monto_base = 0

cout "por favor ingrese el numero de hijos que tiene"

cin num_hijos

if num_hijos <= 2;

   monto_base = 70.00

if num_hijos <= 5:

   monto_base = 90.00

else:

   monto_base = 120.00

for edad in edades_escolares:

    if 6 <= edad <= 18:
    monto_base <= 10.00

if es_viuda:

   monto_base + 20.00

   monto_total = calcularSubsidio (num_hijos,edades_escolares, es_viuda)

   cout ( "el monto mensual que recibirira la familia es de Q." monto_total)


    return 0;
}
```


## Ejercicio 2: 
escribir una aplicación que solicite al usuario un número que será la longitud de dos
vectores que se deben llenar aleatoriamente, sume los valores e indique si ocurre cualquiera de los
siguientes escenarios. a) Son iguales, b) vector A es menor a B, c) vector B es menor a A
### CODIGO 1

```C++
//calcular longitud de vectores

#include <iostream>

using namespace std;

int main {

int longitud;

cout << "ingrese la longitud de los vectores: " ;

cin >> longitud;

srand(time(0));

vector<int> vectorA;

vecor<int> vectorB;

for ( int i = 0; 1 < longitud; i++ ) {

    vectorA.push_back(rand() % 100);

    vectorB.push_back(rand() % 100);

}
    return 0;
}
```


## EJERCICIO 3 
 en estadística descriptiva, se define el rango de un conjunto de datos reales como la
diferencia entre el mayor y el menor de los datos.
Por ejemplo, si los datos son: [5.96, 6.74, 7.43, 4.99, 7.20, 0.56, 2.80], entonces el rango es 7.43 − 0.56
= 6.87.
Escriba un programa que:
a) Pregunte al usuario cuántos datos serán ingresados,
b) Pida al usuario ingresar los datos uno por uno, y
Entregue como resultado el rango de los datos
### CODIGO 3
```C++
//define rango de un conjunto 
#include <iostream>
using namespace std;

int main {

int NumDatos;

cout << "ingrese cuantos datos desea ingresar por favor: ";

cin >> NumDatos

vecor<double> datos;

for (int i = 0; i < NumDatos; i++){

    double dato;
    cout << "ingrese el dato " << i + 1 << ": ";
    cin >> dato;
    datos.push_back (dato);

}

double maximo = max_element ( datos.begin(), datos.end ());

double minimo = min_element(datos.begin(), datos.end ());

double rango = maximo - minimo;

cout << "el rango de los datos es: " << rango <<;

    return 0;
}
```

# EJERCICIO4
Ejercicio 4: solicite al usuario ingresar un número que será el lado de un cuadrado y escriba un
programa que dibuje dicho cuadrado de la siguiente manera: suponga que el usuario ingresó 4

## CODIGO 4
```c++
//cuantos punto quieres en tu cuadrado?

#include <iostream>
using namespace std;

int main () {
int lado;
cout <<"ingrese cuantos puntos quiere en su cuadro";
cin >> lado;

for (int i = 0; i < lado; i++) {
    for (int j = 0; j < lado; j++ ){
        if ( i == 0 || i == lado - 1 || j == 0 || j == lado - 1 ) {
            cout << "*";
        } else { 
            cout << " ";

        }

     }
    cout << endl;
}

    return 0;
}
```
