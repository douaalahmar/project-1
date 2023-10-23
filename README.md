# project-1 //EFFACER LES LANCS PAR DUPLICATION D'UNE CHAINE//
===========================================================================================================================
#include <stdio.h>
#include <string.h>

void main(){
    char ch[100],ch2[100];
    int i=0, j=0,  k=0,;//k est pour suivre les espaces ou les tabulations consecutifs
//saisie d'une chaine ch      
     printf("donner une chaine ch :\n");
     gets(ch);
//supprimer les espaces consecutifs et les tabulations en les remplacant par un seul espace      
     for (i=0;i<strlen(ch);i++){
         if (ch[i]!=' '&& ch[i]!='\t'){
                      ch2[j]=ch[i];
                      j=j+1;
                      k=0;}
         else {
              if (k==0){
              ch2[j]=' ';
              j=j+1;
              k=1;} }    
     printf("la chaine devient:%s\n",ch2); 
     } 
================================================================================================================================
