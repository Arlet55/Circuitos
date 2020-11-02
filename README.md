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
    scanf("%c", &C1);
    printf("Escriba su segunda calificacion:\n");
    fflush( stdin );
    scanf("%c", &C2);
    printf("Escriba su tercer calificacion:\n");
    fflush( stdin );
    scanf("%c", &C3);

    if (C1=='A'||C1=='a')
    {
        calif1=10;

    }
    else if (C1=='B'||C1=='b')
    {
        calif1=9;
    }
    else if (C1=='C'||C1=='c')
    {
        calif1=8;
    }
    else if (C1=='D'||C1=='d')
    {
        calif1=7;
    }
    else if (C1=='E'||C1=='e')
    {
        calif1=6;
    }
    else
    {
        printf ("Su primer calificacion es menor de 6\n");
    }

    if (C2=='A'||C2=='a')
    {
        calif2=10;

    }
    else if (C2=='B'||C2=='b')
    {
        calif2=9;
    }
    else if (C2=='C'||C2=='c')
    {
        calif2=8;
    }
    else if (C2=='D'||C2=='d')
    {
        calif2=7;
    }
    else if (C2=='E'||C2=='e')
    {
        calif2=6;
    }
    else
    {
        printf ("Su segunda calificacion es menor de 6\n");
    }

       if (C3=='A'||C3=='a')
    {
        calif3=10;

    }
    else if (C3=='B'||C3=='b')
    {
        calif3=9;
    }
    else if (C3=='C'||C3=='c')
    {
        calif3=8;
    }
    else if (C2=='D'||C3=='d')
    {
        calif3=7;
    }
    else if (C3=='E'||C3=='e')
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


//Elaboro: Arlet Sanchez Rivera 
    //13 de Octubre 2020
    //0.5 Primer tabla 
    
    #include <stdio.h>

    int main()
    {
    int cont=0;
    int N;

    printf("Escribe el valor de N: ");
    scanf("%d",&N);

    while (cont<=N){

    printf("%d \n",(N*N)-2*cont);
    cont++;
    }
    return 0;
    }
    
    
//Elaboro: Arlet Sanchez Rivera 
    //13 de Octubre 2020
    //0.6 Segunda tabla  
    
    #include <stdio.h>

    int main()
    {
    int cont=0;
    int A, N;

    printf("Escribe el valor de N ");
    scanf("%d", &N);

    while(cont<=(N+(N+1))){

    A=cont;
    printf("%d \n",(3*N)+2*A);
    cont=cont+1;
    }
    return 0;
    }

//Elaboro: Arlet Sanchez Rivera
    //2 de Noviembre 2020
    //0.7 Menu
        
    #include <stdio.h>

    int main()
    {
    int opc=1;

    while (opc!=3)
    {

    printf("**********MENU***********\n");
    printf("\n1.Figuras con asteristicos \n2.Valor de pi \n3.Series\n ");
    printf ("\n ¿Que programa quieres realizar? Elige una opcion\n");
    scanf("%i",&opc);
    system("cls");

    if(opc==1)
    {
    int na=1; //Numero de asteriscos
    int ne=9; //Numero de espacios
    int ia=1; //Incremento de asteriscos
    int ie=1; //Incremento de espacios

    printf ("A)\n");
    for (int r=1;r<=10;r++)//Renglones
    {
        for (int a=1;a<=r;a++)//Asteriscos
        {
            printf ("*");
        }
        printf ("\n");
    }
    printf ("B)\n");
    for (int r=1;r<=10;r++)//Renglones
    {
        for (int a=r;a<=10;a++)//Asteriscos
        {
            printf ("*");
        }
        printf ("\n");
    }
     printf ("C)\n");
    for (int r=1;r<=10;r++)//Renglones
    {
        for (int e=2;e<=r;e++)//Espacios
        {
            printf (" ");
        }
        for (int a=10;a>=r;a--)//Asteriscos
        {
            printf ("*");
        }
        printf ("\n");
    }
        printf ("D)\n");
    for (int r=1;r<=10;r++)//Renglones
    {
        for (int e=9;e>=r;e--) //Espacios
        {
            printf(" ");
        }
        for (int a=1;a<=r;a++)
        {
            printf("*");
        }
        printf ("\n");
    }
        ne=ne+ie;
        na=na+ia;

    return 0;
    }
    
     else if(opc==2)
      {
     int i,n,a = 1;
        float pi = 0, pii;
        printf("Escribe el numero de valores: ");
        scanf("%d",&n);
        for (i=0;i<n;i++)
        {
          pii=4/(float)a;
               if (i % 2 == 1)
               {
                  pi-=pii;
               }
               else
               {
                   pi+=pii;
               }
          a += 2;
        }
    printf("El valor de Pi es: %.3f", pi);
    return 0;
     }
     
     else if (opc==3)
       {
        int N, P, S, T, C;
        printf ("Escribe el numero de digitos que deseas ver\n");
        scanf ("%d",&N);
        P=0;
        S=0;
        T=0;
        C=0;
    printf ("\na):");
    while (P<=N)
    {
        int n=-1;
        for (P=1;P<=N;P++)
        {
            n=n+2;
            printf ("%d, ",n);
        }
    }
    printf ("\nb):");
    while (S<=N)
    {
        int n=-1;
        for (S=1;S<=N;S++)
        {
            n=n+3;
            printf ("%d, ",n);
        }
    }
    printf ("\nc):");
    while (T<=N)
    {
        int n=40;
        for (T=1;T<=N;T++)
        {
            n=n-10;
            printf ("%d, ",n);
        }
    }
    printf ("\nd):");
    while (C<=N)
    {
        int n=7;
        for (C=1;C<=N;C++)
        {
            n=n+8;
            printf ("%d, ",n);
        }
    }
    return 0;
    }
    }
    }
