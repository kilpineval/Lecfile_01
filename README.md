#include<studio.h>
#include<string.h>

int main(){
  FILE * ptr;
  char archivo[80] = "expresion.txt";
  char cadena;
  int i;
  ptr = fopen(archivo, w);
  if(ptr){
    printf("El archivo es de tipo '\%s\` se abrio de manera correcta \n");
    
  }else{
    printf("Error al abrir el archivo \n);
    return 1;
  }
}
