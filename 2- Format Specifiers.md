they specify how a value should be read or displayed
with them we can set       **width**   ,     **precision**      ,     **flags(+)**     of a value

### `"%d"` and width and flags
---

```c
#include <stdio.h>
int main(){

int x = 3;
printf("%d\n",x);     //   3         
        
printf("%4d\n",x);    //   four space than 3        (width)
printf("%-4d\n",x);   //   3 then four space        (width)

printf("%+d\n",x);    //   +3                       (falgs)
printf("%-d\n",x);    //   3

printf("%04d\n",x);

return 0;
}
``` 

```
3
   3
3  
+3
3
0003
```

> `printf("%-d",x);` this statement prints  3
> `printf("%-4d",x);` this statements prints 3 then four space


### `"%f"` and  precision
---
`"%f"` after . it shows 6 digit 
`"%.2f"` after . it shows 2 digit

```c
#include <stdio.h>
int main() {

float x = 4.5f;
printf("%f\n",x);
printf("%.3f",x);

return 0;
}
```

```
4.500000
4.500
```

