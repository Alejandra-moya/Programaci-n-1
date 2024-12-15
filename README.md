#include <iostream> // Librería estándar para entrada/salida
using namespace std;

int main() {
    int numeros[10]; // Array para almacenar los 10 números ingresados
    // Variables para contar las frecuencias
    int freq1 = 0, freq2 = 0, freq3 = 0, freq4 = 0, freq5 = 0;
    // Solicitar al usuario ingresar los 10 números
    cout << "Por favor, ingresa 10 numeros enteros entre los valores de 1 y 5:" << endl;
    for (int i = 0; i < 10; i++) {
        cout << "Numero " << i + 1 << ": ";
        cin >> numeros[i];
        // Validar que el número esté en el rango [1, 5]
        while (numeros[i] < 1 || numeros[i] > 5) {
            cout << "Numero invalido. Por favor, ingresa un numero entre los valores de 1 y 5: ";
            cin >> numeros[i];
        }
    }
    // Contar las frecuencias
    for (int i = 0; i < 10; i++) {
        switch (numeros[i]) {
            case 1: freq1++; break;
            case 2: freq2++; break;
            case 3: freq3++; break;
            case 4: freq4++; break;
            case 5: freq5++; break;
        }
    }
    // Mostrar los resultados
    cout << "\nFrecuencia de los numeros ingresados:" << endl;
    cout << "Numero 1: " << freq1 << " veces" << endl;
    cout << "Numero 2: " << freq2 << " veces" << endl;
    cout << "Numero 3: " << freq3 << " veces" << endl;
    cout << "Numero 4: " << freq4 << " veces" << endl;
    cout << "Numero 5: " << freq5 << " veces" << endl;


    return 0;
}
![image](https://github.com/user-attachments/assets/23b53d09-50b3-4e48-909b-482a7f75bccb)
