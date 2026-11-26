### 1- `for` loop

```c
for(initialization; condition; update){
	line 1
	line 2
}
```

```c
for(int i = 0; i<10; i++,j++){
    line 1
    line 2
}
```

##### EX-1
```c
#include <stdio.h>
int main(){ 

    for(int i = 0; i<10; i++){
        printf("%d",i);
    }
    
    return 0;
}
```

```
0123456789
```


### 2- infinite `for` loop

```c
for(;;){
    line 1
    line 2
   }
```



