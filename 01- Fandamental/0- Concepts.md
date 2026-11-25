### whitespace
refers to characters that represent spaces
> like : space, \n, \t, ...

### Variable Scops
refers to where a variable is recognized and accessible 
variables can be same name if they are in different scops `{}`

```c
#include <stdio.h>

int var = 2; // GLOBAL SCOPE (hard to debug) because every local scope has access


int function(){
int x = 2;   // Local scope 
}

int main(){
int x = 3;  // Local scope

return 0;
}
```
