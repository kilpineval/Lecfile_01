#include<studio.h>
#include<string.h>

int main(){
  FILE * ptr;
  char archivo[80] = "expresion.txt";
  char cadena[90] = "esto necesita practica";
  int i;
  ptr = fopen(archivo, w);
  if(ptr){
    printf("El archivo es de tipo '\%s\'  se abrio de manera correcta \n");
                                     
    
  }else{ 
    printf("Error al abrir el archivo \n);
    return 1;
    
  }
  do{
    gets(cadena);
    
    fprintf(ptr, "%s, \n",cadena);
    printf("Escriba la expresion que ud. desea y luego retorno para finalizar \n);
  }while(strcmp(cadena, "") !=0);
  fclose(ptr);
  printf("vamos a leer la expresion que has escrito \n");
  ptr=fopen(archivo, "r");
  if(ptr){
    printf("El archivo se abrio de manera correcta, \n);
    
  }else{
    printf("el arcrivo no se abrio por alguna razon \n")
  }
  
  
  printf("Escribe la expresion que ud. desea y luego retorno para finalizar \n );
  
  
  
}
