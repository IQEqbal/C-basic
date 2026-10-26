## comment

### //
```c 
#include <stdio.h>
int main(){
// this a line comment
return 0;
}
```
### /*       */
```c
#include <stdio.h>
int main(){
/* this is a
 multiline comment */
return 0;
}

```

## Data Types and their Format specifiers

> Format specifiers : they specify how a value should be read or displayed

### int  /  %d
`int x = 5;`

```c
#include <stdio.h>
int main(){

int x = 5;
printf("x = %d",x);
return 0;
}
```

```
x = 5
```

### float / %f
`flout x = 45.4;`
`flout x = 45.4f;`

```c
#include <stdio.h>
int main(){

float x = 45.4;
float y = 45.4f;
printf("x = %f \n" ,x);
printf("y = %f \n" ,y);
return 0;
}
```

```
x = 45.400002 
y = 45.400002 
```

### double / %lf
`double pi = 3.143432343;`

```c
#include <stdio.h>
int main(){

double pi = 3.143432343;
printf("pi = %lf",pi);
return 0;
}
```

```
pi = 3.143432
```

### char / %c
`char symbol = 'A';`

```c
#include <stdio.h>
int main(){

char currency = '$';
printf("%c",currency);
return 0;
}
```

```
A
```

### String / %s
`char name[] = "somthing";`
`char name[a] = "somthing";`

to  declaring we must write `char name[a];` 


```c
#include <stdio.h>
int main(){

char name[] = "Eqbal";
printf("%s",name);
return 0;
}
```

```
Eqbal
```

### bool / %d
`#include <stdbool.h>`
`bool ciondition = true;`

```c
#include <stdio.h>
#include <stdbool.h>
int main(){

bool isOnline = false;
printf("%d",isOnline);
return 0;
}
```

```
0
```