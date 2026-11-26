
#### EX-1
```c
#include <stdio.h>
#include <string.h>
int main(){

    char name[50] = "";
    int lenght = 0;

    printf("Enter your name :");
    fgets(name,sizeof(name),stdin);
    name[strlen(name)-1] = '\0';
    lenght = strlen(name);


    for(int i = 0; i < lenght; i++){
        for(int j = 0; j< i; j++){
            printf("%c",name[j]);
        }
        printf("\n");
    }
    
    
    for(int i = lenght; i >= 0; i--){
        for(int j = 0; j <i; j++){
            printf("%c",name[j]);
        }
        printf("\n");
    }


    return 0;
}
```

```
M
Mo
Moh
Moha
Moham
Mohamm
Mohamma
Mohammad
Mohammad 
Mohammad E
Mohammad Eq
Mohammad Eqb
Mohammad Eqba
Mohammad Eqbal
Mohammad Eqba
Mohammad Eqb
Mohammad Eq
Mohammad E
Mohammad 
Mohammad
Mohamma
Mohamm
Moham
Moha
Moh
Mo
M
```

#### EX-2
```c
#include <stdio.h>
int main(){  

// Lower triangular
for(int i = 10; i>=0; i--){

    // Distance triangular
    for(int k = 0; k < i; k++){
        printf(" ");
    }  
    
    for(int j = i; j<=10; j++){  
        printf("*");
    }

    for(int h = i; h < 10; h++){
        printf("*");
    }
    printf("\n");
}


// Upper triangular
for(int ii = 0; ii<11; ii++){ 

    // Distance triangular
    for(int kk = ii; kk > 0; kk--){
        printf(" ");
    }  

    for(int jj = 10; jj >= ii; jj--){
       printf("*");
    }

     for(int jj = 10; jj > ii; jj--){
       printf("*");
    }
    printf("\n"); 

}
    return 0;
}
```

```
          *
         ***
        *****
       *******
      *********
     ***********
    *************
   ***************
  *****************
 *******************
*********************
*********************
 *******************
  *****************
   ***************
    *************
     ***********
      *********
       *******
        *****
         ***
          *
```