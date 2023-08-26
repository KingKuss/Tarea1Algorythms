# Tarea1Algorythms
# Algoritmos de Conversión de Medidas

En este repositorio, se presentan tres implementaciones de algoritmos para convertir medidas en distintos lenguajes: C++, Python y Pseudocódigo.

## C++ - Convertidor de Medidas

```cpp
#include <iostream>

using namespace std;

int main()
{

    //Declarar Variables CM para la medida del usuario, RES que sera el resultado y OP para la opcion
    float fltCM,fltRES;
    char OP;
    

    //Estructura
    cout << "Bienvenido al convertidor de medidas \n";
    cout << "Por favor ingrese una medida en centimetros \n";
    cin >> fltCM;
    cout << "Seleccione a que medida desea convertir en mayusculas\n";
    cout << "Metros (M)\n";
    cout << "Yardas (Y)\n";
    cout << "Varas (V)\n";
    cout << "Pulgadas (P)\n";
    cout << "Pies (F)\n";
    cin >> OP;

    if (OP == 'M'|| OP == 'm') {
        fltRES = fltCM / 100;
        cout << "La medida en metros es: " << fltRES << " Mts";
    }
    else if (OP == 'Y'|| OP == 'y') {
        fltRES = fltCM / 91.44;
        cout << "La medida en yardas es: " << fltRES << " Yd";
    }
    else if (OP == 'V'|| OP == 'v') {
        fltRES = fltCM / 83.33;
        cout << "La medida en varas es: " << fltRES << " Varas";
    }
    else if (OP == 'P'||OP == 'p') {
        fltRES = fltCM / 2.54;
        cout << "La medida en pulgadas es: " << fltRES << " In";
    }
    else if (OP == 'F'|| OP == 'f') {
        fltRES = fltCM / 30.48;
        cout << "La medida en pies es: " << fltRES << " Ft";
    }
    else {
        cout << "No ingresaste una opción disponible";
    }

    cout << "Gracias por utilizar el algoritmo\n";

    return 0;
}
```
## Python - Convertidor de medidas
```python
def main():
    # Declarar Variables: fltCM para la medida del usuario, fltRES que será el resultado, y OP para la opción
    fltCM = float(input("Por favor ingrese una medida en centímetros: "))
    fltRES = 0.0
    OP = input("Seleccione a qué medida desea convertir en mayúsculas:\n"
               "Metros (M)\n"
               "Yardas (Y)\n"
               "Varas (V)\n"
               "Pulgadas (P)\n"
               "Pies (F)\n")

    if OP == 'M' or OP == 'm':
        fltRES = fltCM / 100
        print(f"La medida en metros es: {fltRES:.2f} Mts")
    elif OP == 'Y' or OP == 'y':
        fltRES = fltCM / 91.44
        print(f"La medida en yardas es: {fltRES:.2f} Yd")
    elif OP == 'V' or OP == 'v':
        fltRES = fltCM / 83.33
        print(f"La medida en varas es: {fltRES:.2f} Varas")
    elif OP == 'P' or OP == 'p':
        fltRES = fltCM / 2.54
        print(f"La medida en pulgadas es: {fltRES:.2f} In")
    elif OP == 'F' or OP == 'f':
        fltRES = fltCM / 30.48
        print(f"La medida en pies es: {fltRES:.2f} Ft")
    else:
        print("No ingresaste una opción disponible")

    print("Gracias por utilizar el algoritmo")

if __name__ == "__main__":
    main()

```
## Pseudocodigo - Convertidor de medidas
```Pseudocode
Algoritmo ConvertidorDeMedidas
	
    Definir fltCM, fltRES Como Real
    Definir OP Como Carácter
	
    Escribir "Bienvenido al convertidor de medidas"
    Escribir "Por favor ingrese una medida en centímetros"
    Leer fltCM
    Escribir "Seleccione a qué medida desea convertir en mayúsculas"
    Escribir "Metros (M)"
    Escribir "Yardas (Y)"
    Escribir "Varas (V)"
    Escribir "Pulgadas (P)"
    Escribir "Pies (F)"
    Leer OP
	
    Si OP = 'M' o OP = 'm' Entonces
        fltRES <- fltCM / 100
        Escribir "La medida en metros es:", fltRES, " Mts"
    Sino
        Si OP = 'Y' o OP = 'y' Entonces
            fltRES <- fltCM / 91.44
            Escribir "La medida en yardas es:", fltRES, " Yd"
        Sino
            Si OP = 'V' o OP = 'v' Entonces
                fltRES <- fltCM / 83.33
                Escribir "La medida en varas es:", fltRES, " Varas"
            Sino
                Si OP = 'P' o OP = 'p' Entonces
                    fltRES <- fltCM / 2.54
                    Escribir "La medida en pulgadas es:", fltRES, " In"
                Sino
                    Si OP = 'F' o OP = 'f' Entonces
                        fltRES <- fltCM / 30.48
                        Escribir "La medida en pies es:", fltRES, " Ft"
                    Sino
                        Escribir "No ingresaste una opción disponible"
                    FinSi
                FinSi
            FinSi
        FinSi
    FinSi
	
    Escribir "Gracias por utilizar el algoritmo"
	
FinAlgoritmo

```
