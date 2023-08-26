**pseudocódigo**

Algoritmo Conversión_de_Longitud
    
    Definir centimetros, resultado como Real
    Definir unidad_destino como Cadena
    
    Escribir "Ingrese la longitud en centímetros:"
    Leer centimetros

    Escribir "Seleccione la unidad a la que desea convertir (metros, yardas, varas, pulgadas, pies):"
    Leer unidad_destino

    Si unidad_destino = "metros" Entonces
        resultado = centimetros / 100  // Dividimos por 100 para convertir a metros.
    Sino Si unidad_destino = "yardas" Entonces
        resultado = centimetros / 91.44  // Dividimos por 91.44 para convertir a yardas.
    Sino Si unidad_destino = "varas" Entonces
        resultado = centimetros / 50.8  // Dividimos por 50.8 para convertir a varas.
    Sino Si unidad_destino = "pulgadas" Entonces
        resultado = centimetros / 2.54  // Dividimos por 2.54 para convertir a pulgadas.
    Sino Si unidad_destino = "pies" Entonces
        resultado = centimetros / 30.48  // Dividimos por 30.48 para convertir a pies.
        Sino
        Escribir "Unidad de destino no válida"
        Detener
    Fin Si
    


    Escribir "El resultado es:", resultado, unidad_destino
    Fin Algoritmo
    
**C++**
#include <iostream>
#include <string>
using namespace std;

int main() {
    float centimetros, resultado;
    string unidad_destino;

    cout << "Ingrese la longitud en centímetros: ";
    cin >> centimetros;  // Usamos 'cin' para leer el valor ingresado por el usuario.

    cout << "Seleccione la unidad a la que desea convertir (metros, yardas, varas, pulgadas, pies): ";
    cin >> unidad_destino;  // Usamos 'cin' para leer la unidad de destino ingresada.

    if (unidad_destino == "metros") {
        resultado = centimetros / 100;  // Dividimos por 100 para convertir a metros.
    } else if (unidad_destino == "yardas") {
        resultado = centimetros / 91.44;  // Dividimos por 91.44 para convertir a yardas.
    } else if (unidad_destino == "varas") {
        resultado = centimetros / 50.8;  // Dividimos por 50.8 para convertir a varas.
    } else if (unidad_destino == "pulgadas") {
        resultado = centimetros / 2.54;  // Dividimos por 2.54 para convertir a pulgadas.
    } else if (unidad_destino == "pies") {
        resultado = centimetros / 30.48;  // Dividimos por 30.48 para convertir a pies.
    } else {
        cout << "Unidad de destino no válida" << endl;
        return 1;
    }
    cout << "El resultado es: " << resultado << " " << unidad_destino << endl;  // Mostramos el resultado.
    return 0;
    }


**PY**

centimetros = float(input("Ingrese la longitud en centímetros: "))  # Usamos 'input' para obtener el valor ingresado como cadena y luego lo convertimos a flotante.

unidad_destino = input("Seleccione la unidad a la que desea convertir (metros, yardas, varas, pulgadas, pies): ")  # Usamos 'input' para obtener la unidad de destino ingresada.

if unidad_destino == "metros":
    resultado = centimetros / 100  # Dividimos por 100 para convertir a metros.
elif unidad_destino == "yardas":
    resultado = centimetros / 91.44  # Dividimos por 91.44 para convertir a yardas.
elif unidad_destino == "varas":
    resultado = centimetros / 50.8  # Dividimos por 50.8 para convertir a varas.
elif unidad_destino == "pulgadas":
    resultado = centimetros / 2.54  # Dividimos por 2.54 para convertir a pulgadas.
elif unidad_destino == "pies":
    resultado = centimetros / 30.48  # Dividimos por 30.48 para convertir a pies.
else:
    print("Unidad de destino no válida")
    exit(1)

print("El resultado es:", resultado, unidad_destino)  # Mostramos el resultado.
    
    
