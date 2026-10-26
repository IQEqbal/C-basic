`#include <math.h>`


| Function     | usage                    | output |
| ------------ | ------------------------ | ------ |
| `sqrt(var)`  | square                   | double |
| `pow(var,a)` | var^a                    | double |
| `round(var)` | roundoff                 | double |
| `ceil(var)`  | Ex: `3.14 --> 3.000000`  | double |
| `floor(var)` | Ex: `3,14 --> 4.0000000` | double |
| `abs(var)`   | \|var\|                  | int    |
| `log(var)`   | logarithm                | double |

```c
#include <stdio.h>
#include <math.h>  

int main(){
    
printf("%f\n",sqrt(9));
printf("%f\n",pow(2,4));
printf("%f\n",round(2.4654321));
printf("%d\n",abs(-3));

return 0;
}
```

```
3.000000
16.000000
2.000000
3
```

