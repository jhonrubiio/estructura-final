# Proyecto 1 - Basket

**Un juego de basketball se juega en cuatro tiempos, participan dos equipos y cada equipo posee 5 jugadores. Suponiendo que no haya cambios de jugadores, escriba un programa que sea capaz de almacenar los puntos encestados por cada jugador de cada equipo en cada tiempo. Estos puntos deben acumularse para cada uno de los jugadores de cada equipo en cada tiempo y luego imprimir los resultados del juego en cada tiempo para cada jugador. Las lecturas deben hacerse en un ciclo y este ciclo debe terminar cuando se digite el tiempo número 5.Y gana el equipo que tenga más puntos. Si al final del 5to tiempo hay empate, se va a tiempo extra y dicho tiempo extra será hasta el infinito. Este tiempo extra acabará cuando ya no haya jugadores disponibles en condición física CREATIVIDAD y MUCHO ESMERO.**


#include <stdio.h>
#include <stdlib.h>
#include <conio.h>
#include <time.h>
#include <dos.h>

int main (void)
{
    int LebronTGL,PedroTGL,JuanTGL,AntonioTGL,EmilioTGL,TGL; // jugadores del equipo 1 TGL = Tigres del Licey
    int DavidAGC,JavierAGC,MarioAGC,SergioAGC,MarcosAGC,AGC; // jugaores del equipo 2 AGC = Aguilas Cibaeñas
    
    printf("  ----------------Final del Campeonato Nacional de Baloncesto 2019----------------\n\n");
    
    LebronTGL = rand () % 60;
    PedroTGL = rand () % 44;
    JuanTGL = rand () % 44;  //Se aplican los valores de los puntos anotados por cada jugador
    AntonioTGL = rand () % 50;
    EmilioTGL = rand () % 36;
    
    DavidAGC = rand () % 60;
    JavierAGC = rand () % 44;
    MarcosAGC = rand () % 44;  //Se aplican los valores de los puntos anotados por cada jugador
    MarioAGC = rand () % 50;
    SergioAGC = rand () % 36;
    
    printf("\tLebron TGL %i\t\t",LebronTGL);
    printf("\tDavid AGC %i\n",DavidAGC);
    printf("\tPedro TGL %i\t\t",PedroTGL);
    printf("\tJavier AGC %i\n",JavierAGC);
    printf("\tJuan TGL %i\t\t",JuanTGL);
    printf("\tMarcos AGC %i\n",MarcosAGC);        //Se imprimen los puntos de cada jugador de manera aleatoria
    printf("\tAntonio TGL %i\t\t",AntonioTGL);
    printf("\tMario AGC %i\n",MarioAGC);
    printf("\tEmilio TGL %i\t\t",EmilioTGL);
    printf("\tSergio AGC %i\n\n",SergioAGC);
    
    TGL = LebronTGL + PedroTGL + JuanTGL + AntonioTGL + EmilioTGL;
    AGC = DavidAGC + JavierAGC + MarioAGC + SergioAGC + MarcosAGC;
    printf("\tTigres del Licey %i\t",TGL);
    printf("\tAguilas Cibaeñas %i\n",AGC);
 
       long int i=0;
   clock_t comienzo;
 
   comienzo=clock();
   
 
   printf( "Numeros de segundos transcurridos desde el comienzo del programa: %f s\n", (clock()-comienzo)/(double)CLOCKS_PER_SEC );
    return 0;
}

      
