//Elaboro: Arlet Sanchez Rivera 
   //24 de Septiembre 2020
   //0.1 Calculo de resistencias de leds

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
    
//Elaboro: Arlet Sanchez Rivera 
    //24 de Septiembre 2020
    //0.2 Calculo de la corrientes y resistencias 
    
    #include <stdio.h>

    int main (){

    float V; //valor de la fuente en volts
    int R1, R2, R3; //valor de las resistencias
    float I1,I2, I3; // valor de la corriente en cada resistencia

    printf ("Escribe el valor de la fuente V: ");
    scanf("%f",&V);

    printf("El valor debe ser escrito en notacion completa no usar prefijos\n");
    printf ("Resistencia 1: ");
    scanf("%d", &R1);
    printf ("Resistencia 2: ");
    scanf("%d", &R2);
    printf ("Resistencia 3: ");
    scanf("%d", &R3);

    I1= V/R1;
    I2= V/R2;
    I3= V/R3;

    printf("La corriente I1 es %0.3fA\n",I1);
    printf("La corriente I2 es %0.3fA\n",I2);
    printf("La corriente I3 es %0.3fA\n",I3);
    printf("El voltaje en R1 es %0.3fV\n", V);
    printf("El voltaje en R2 es %0.3fV\n", V);
    printf("El voltaje en R3 es %0.3fV\n", V);

    }
    
    
//Elaboro: Arlet Sanchez Rivera
    //1 de Octubre 2020
    //0.3 Calificaciones 
    
    #include <stdio.h>

    main()
    {
    char  C1, C2, C3;
    float prom, calif1, calif2, calif3;
    printf("Escriba sus tres calificaciones, recordando que se deben escribir en letra mayuscula usando A, B, C, D o E\n");
    printf("Escriba su primer calificacion:\n");
    printf("Escriba su segunda calificacion:\n");
    printf("Escriba su tercer calificacion:\n");
    scanf("%c %c %c", &C1, &C2, &C3);

    if (C1=='A')
    {
        calif1=10;
    }
    else if (C1=='B')
    {
        calif1=9;
    }
    else if (C1=='C')
    {
        calif1=8;
    }
    else if (C1=='D')
    {
        calif1=7;
    }
    else if (C1=='E')
    {
        calif1=6;
    }
    else
    {
        printf ("Su primer calificacion es menor de 6\n");
    }

    if (C2=='A')
    {
        calif2=10;
    }
    else if (C2=='B')
    {
        calif2=9;
    }
    else if (C2=='C')
    {
        calif2=8;
    }
    else if (C2=='D')
    {
        calif2=7;
    }
    else if (C2=='E')
    {
        calif2=6;
    }
    else
    {
        printf ("Su segunda calificacion es menor de 6\n");
    }

       if (C3=='A')
    {
        calif3=10;
    }
    else if (C3=='B')
    {
        calif3=9;
    }
    else if (C3=='C')
    {
        calif3=8;
    }
    else if (C2=='D')
    {
        calif3=7;
    }
    else if (C3=='E')
    {
        calif3=6;
    }
    else
    {
        printf ("Su tercer calificacion es menor de 6\n");
    }

    prom=(calif1+calif2+calif3)/3;
    printf ("Su promedio es de:%f\n", prom);

    }
    
    
//Elaboro: Arlet Sanchez Rivera 
    //1 de Octubre 2020
    //0.4 Ecuacion cuadratica 
    
    #include <stdio.h>
    #include <math.h>

    int main () {
    int a, b, c, d;
    float x, y;

    printf("Resolucion de ecuaciones de segundo grado \n");
    printf("Escribe el valor de a: ");
    scanf("%d",&a);

    printf("Escribe el valor de b: ");
    scanf("%d",&b);

    printf("Escribe el valor de c: ");
    scanf("%d",&c);

    d = (b*b)-(4*a*c);
    if (d>0) {
        x = (-b+sqrt(d))/(2*a);
        y = (-b-sqrt(d))/(2*a);

        printf("El valor de x1 = %f\n",x);
        printf("El valor de x2 = %f\n",y);
    }

    else if (d==0) {
        x =(-b)/(2*a);
        printf("x1 = %.2f\n",x);
    }

    else{
        printf("La ecuacion no tiene solucion");
    }

    return 0;
    }

