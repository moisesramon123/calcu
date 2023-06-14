#include <iostream>

using namespace std;

int main() {
    float num1, num2, resultado;
    char operador;

 
    cout << "Ingrese un operador (+, -, *, /): ";
    cin >> operador;
    
       cout << "Ingrese numero: ";
    cin >> num1;


    cout << "Ingrese numero: ";
    cin >> num2;
     switch (operador) {
        case '+':
            resultado = num1 + num2;
            cout << "la suma es: " << resultado << endl;
            break;
        case '-':
            resultado = num1 - num2;
            cout << " la resta es: " << resultado << endl;
            break;
        case '*':
            resultado = num1 * num2;
            cout << " la multiplicacion es: " << resultado << endl;
            break;
        case '/':
            if (num2 != 0) {
                resultado = num1 / num2;
                cout << " la división es: " << resultado << endl;
            } else {
                cout << "No se puede dividir." << endl;
            }
            break;
        default:
            cout << "Operador inválido." << endl;
            break;
    }

    return 0;
}
