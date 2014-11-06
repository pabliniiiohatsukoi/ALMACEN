#include <iostream>
#include <stdio.h>
#include <stdlib.h>
#include "productos.h"
#include "tallarines.h"
#include "leche.h"
#include "cereales.h"

using namespace std;

int main()
{
    Productos P;
    Tallarines T;
    Cereales C;
    Leche L;
    int opcion=1;
    while(opcion!=0){
    cout << "Menu" << endl << endl;
    cout << "1- llenar stock de tallarines" << endl;
    cout << "2- mostrar tallarines" << endl;
    cout << "3- llenar stock de cereales" << endl;
    cout << "4- mostrar cereales" << endl;
    cout << "5- llenar stock de leche" << endl;
    cout << "6- mostrar leche" << endl;
    cout << "7- comprar tallarines" << endl;
    cout << "8- comprar leche " << endl;
    cout << "9- comprar cereales" << endl;
    cout << "0- salir" << endl;
    cout << " " << endl;
    cin >> opcion;
    switch(opcion){
        case 1:
            cout<<endl;
            fflush(stdin);
            T.setproductos();
            fflush(stdin);
            T.settallarines();
            cout<<endl;
            system("pause");
            system("cls");
            break;
            case 2:
            cout<<endl;
            T.getproductos();
            T.gettallarines();
            cout<<endl;
            system("pause");
            system("cls");
            break;

            case 3:
            cout<<endl;
            fflush(stdin);
            C.setproductos();
            fflush(stdin);
            C.setcereales();
            cout<<endl;
            system("pause");
            system("cls");
            break;

            case 4:
            cout<<endl;
            C.getproductos();
            C.getcereales
            ();
            cout<<endl;
            system("pause");
            system("cls");
            break;
            case 5:
            cout<<endl;
            fflush(stdin);
            L.setproductos();
            fflush(stdin);
            L.setleche();
            cout<<endl;
            system("pause");
            system("cls");
            break;
            case 6:
            cout<<endl;
            L.getproductos();
            L.getleche();
            cout<<endl;
            system("pause");
            system("cls");
            break;
            case 7:
            cout<<endl;
            T.setcompratallarines();
            cout<<endl;
            system("pause");
            system("cls");
            break;
            case 8:
            cout<<endl;
            L.setcompraleche();
            cout<<endl;
            system("pause");
            system("cls");
            break;
            case 9:
            cout<<endl;
            C.setcompracereales();
            cout<<endl;
            system("pause");
            system("cls");
            break;

        case 0:
            return 0;
            break;
    }}

    return 0;
}
