### `getchar()` function
it takes a character from the Input Buffer
```c
#include <stdio.h>
int main(){  

char grade;
char symbol;  

printf("Enter your grade: ");
scanf("%c",&grade);

char x = getchar();

printf("Enter your symbol: ");
scanf(" %c",&symbol);

printf("%c",grade);
printf("%c",symbol);
printf("%c",x);

return 0;
}
```

```
Enter your grade: ab
Enter your symbol: a
aab
```

### `sizeof(var)`
it returns us the length of string
```c
#include <stdio.h>
int main(){

char name[30];
int length = sizeof(name);
printf("%d",length);

return 0;
}
```

```
30
```


## `fgets(Var, size_of_var, stdin);`

`char var[30];`
`fgets(var,30,stdin);`

#### EX-1
```c
#include <stdio.h>
int main(){

char name[50];
printf("Enter your full name: ");
fgets(name,sizeof(name),stdin);

printf("%s",name);
return 0;
}
```

```
Enter your full name: mohammed Eqbal
mohammed Eqbal
```

#### EX-2
```c
#include <stdio.h>
int main(){

char grade;
char name[40];

printf("Enter your grade: ");
scanf("%c",&grade);   // Input Buffer [A,\n]  
                      // Input Buffer [\n]
getchar();           //  Input Buffer []

printf("Enter your name: "); 
fgets(name,sizeof(name),stdin);      // Input Buffer [M,o,h,...,E,q,b,a,l,\n]

printf("%c\n",grade);
printf("%s",name);

return 0;
}
```

```
Enter your grade: A
Enter your name: Mohammad Eqbal
A
Mohammad Eqbal
```