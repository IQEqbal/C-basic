### `while`

```c
while(condition){
    line 1
    line 2
}
```

##### EX-1
```c
#include <stdio.h>
int main(){

int i = 0;
while(i<10){
	printf("%d",i);
	i++;
	}
	
return 0;
}
```

```
0123456789
```


### `do while`
first code is executed then the condition is checked
at least once the block codes of `while` will be executed

```c
do {
	line 1
	line 2
	
}while (condition);
```

```c
#include <stdio.h>
int main(){  

int i = 0;
do {
    printf("%d",i);
    i++;
    
    } while(i <10);

return 0;
}
```

```
0123456789
```