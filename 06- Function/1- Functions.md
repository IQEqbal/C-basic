### `void` Function
to call a function we must use `()`

```c
#include <stdio.h>

void nameFunction(arg1, arg2,..., argn){
	line 1
	line 2
	}

int main(){

return 0;

}
```

#### EX-1
```c
#include <stdio.h>
#include <string.h>
 
void happyBirthDay(char myDear[], int yearsOld){
    printf("Happy birthday %s\n", myDear);
    printf("you are %d years old now", yearsOld); 
}  

int main(){

char name[50];
int age;  

printf("Enter a name: ");
fgets(name,sizeof(name),stdin);
name[strlen(name)-1] = '\0';  

printf("Enter his/her age: ");
scanf("%d",&age); 

happyBirthDay(name, age);              // calling function
return 0;
}
```

```
Enter a name: Eqbal
Enter his/her age: 21
Happy birthday Eqbal
you are 21 years old now
```


### `return` Function
returns a value back to where you call a function 
```c
#include <stdio.h>

returnType nameFunction(arg1, arg2,...,argn){
	line 1
	line 2
	return val;
}

int main(){

return 0;
}
```

#### EX-1
```c
#include <stdio.h>

float square(float x){
    return x * x;
}

double cube(double x){
    return x * x * x;
}  

int main(){

    printf("%lf\n",square(2));
    printf("%lf",cube(3));
    
    return 0;
}
```

```
4.000000
27.000000
```