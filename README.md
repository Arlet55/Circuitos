//Circuitos- Calculo de las resistencias 

#include <stdio.h>

int main (){

    float V, R, l1, l2, l3, l4; //valor de la fuente en volts y los leds

    printf ("Escribe el valor de la fuente V: ");
    scanf("%f",&V);

    l1= (V-2)/0.02;
    l2= (V-1.8)/0.015;
    l3= (V-3)/0.02;
    l4= (V-2.8)/0.02;

    printf("El valor de la resistencia para el led amarillo brillante es %0.03f Ohms\n", l1);
    printf("El valor de la resistencia para el led verde std es %0.03f Ohms\n", l2);
    printf("El valor de la resistencia para el led azul brillante es %0.03f Ohms\n", l3);
    printf("El valor de la resistencia para el led blanco es %0.03f Ohms\n", l4);

    }
