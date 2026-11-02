## `scanf()`
it used to take input from user

`int variable = 0;`
`scanf("%d",&variable);`
`&` allows `scanf()` to access the memory address of the variable 

### Input Buffer 
it a temporary area in memory(RAM) where user input is stored until program reads it
> keyboard --> input buffer --> scanf --> variable

```c
#include <stdio.h>
int main(){

int inputNum = 0;
printf("inter a number: ");
scanf("%d",&inputNum);

printf("%d",inputNum);

return 0;
}
```

> `scanf()` cant read any whitespaces

```c
#include <stdio.h>
int main(){

char name[] ="";
printf("Enter your full name: ");
scanf("%s",name);

printf("\n%s",name);

return 0;
}
```

```
Enter your full name: mohammad Eqbal
mohammad
```

as I write `scanf()` can not read any whitespaces except `sanf("%c"...)` it can read but if we write like `scanf(" %c"...)` this now it can not read though 
#### EX-1
```c
#include <stdio.h>
int main(){

char grade;
char symbol;

printf("Enter your grade: ");
scanf("%c",&grade);

printf("Enter your symbol: ");
scanf("%c",&symbol);        // If scanf(" %c",&symbol);  it works

printf("%c",grade);
printf("%c",symbol);

return 0;
}
```
> it doesn't work 
## Undefined Behavior

```c
#include <stdio.h>
int main(){

int age;
float gpa;
char grade;
char name[30];

printf("%d\n",age);
printf("%f\n",gpa);
printf("%c\n",grade);
printf("%s\n",name);

return 0;
}
```
for each try(run) it become different output
```
75
-270790971878379323578646528.000000

0pδ╩÷
```

### Solution

```c
#include <stdio.h>
int main(){

int age = 0;
float gpa = 0.0f;
char grade = '\0';
char name[30] = "";    // it still take up 30 charaters,(30bytes)

printf("%d\n",age);
printf("%f\n",gpa);
printf("%c\n",grade);
printf("%s\n",name);

return 0;
}
```

```
0
0.000000


```

