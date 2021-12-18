#include <stdio.h>
#include <stdlib.h>
#include <locale.h>



int main()

{
    int opc;
    int p;
    int m;
    int a;
    int op;
    int soma=0;
    #define n 11
    int id[n];
    #define j 33
    int al[j];
    int somam=0;
    float pe[33],menor=99999,mediai,medial;


    do
    {   system("cls");



        printf("\n\n\n\n\n\n\t\t Digite 1 para calcular o peso do jogador mais magro do campeonato ");
        printf("\n\n\n\n\n\n\t\t\ Digite 2 para calcular a media de idade entre os jogadores de cada time ");
        printf("\n\n\n\n\n\n\t\t Digite 3 para calcular a media da altura de todos os jogadores do campeonato ");


        scanf("%d",&opc);



        if(opc==1)
        {   system("cls");
            for(p=0;p<33;p++)
      {

        printf("\n\n Por Favor, Informe o peso do jogador %d: ", (p+1), p);
        scanf("%f",&pe[p]);

           if(menor>pe[p])
           {
               menor=pe[p];
           }
      }
           system("cls");

           printf("\n O Jogador mais leve pesa: %.2f Kg \n\n\n\n ",menor);



            system("pause");
        }

         if(opc==2)
        {
             system("cls");
              for (m=0;m<11;m++)
        {

            printf("Por favor,informe a idade do jogador %d: " , (m+1), m);
            scanf("%d",&id[m]);


               soma= soma + id[m];


        }

            mediai= soma/n;
            system("cls");


            printf("\n\n A media da idade dos jogadores : %.2f \n\n",mediai);
            system("pause");
        }

          if(opc==3)
          {
             system("cls");
             for (a=0;a<33;a++)
        {

            printf("Por favor,informe a altura do jogador %d: " , (a+1), a);
            scanf("%d", &al[a]);


               somam= somam+al[a];


        }

            medial= somam/j;
            system("cls");


            printf("\n\n A media da altura dos jogadores : %.2f \n\n",medial);
            system("pause");
        }
          }while  (opc!=0);
        }




