### String / %s

 `char name[] = "somthing";`
 `char name[a] = "somthing";`
to  declaring we must write `char name[a];` 

in `C` strings are mutable


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

### Accessing to it's index

#### EX-1
```c
#include <stdio.h>
#include <string.h>
int main(){
  
char name[50] = "Eqbal";

printf("%c",name[0]);
printf("%c",name[1]);
printf("%c",name[2]); 

printf("%c",name[-1]);             // Undefined Behavior

return 0;
}
```

```
Eqb
```

#### EX-2
```c
#include <stdio.h>
#include <string.h>
int main(){

char name[50] = "Eqbal";  
name[0] = 'Z';
printf("%s",name);

return 0;
}
```

```
Zqbal
```

### `strlen()`
it returns the length of string

`#include <string.h>`
`strlen(_str);`

```c
#include <stdio.h>
#include <string.h>
int main(){  

char name[50] = "Eqbal";
printf("%d\n",sizeof(name));
printf("%d",strlen(name));

return 0;
}
```

```
50
5
```


### `sizeof()`
it returns us the size of string

`sizeof(_str);`


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


### Notes

* in `c` string always stored `'\0'` at the end
* `'\0'` mean `null` character
* `strlen()` counts characters until `'\0'` 
* `sizeof()` counts the `'\0'` 
```c
#include <stdio.h>
#include <string.h>
int main(){  

char name[] = "Eqbal";
printf("%d\n",strlen(name));
printf("%d",sizeof(name));

return 0;
}
```

```
5
6
```
