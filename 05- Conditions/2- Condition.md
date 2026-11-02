## `switch`

```c
switch (var){
	case val1:
		line 1
		line 2
		break;
		
	case val2:
		line 1
		line 2
		break;
		
	default:
		line 1
		line 2
		break;		
}
```

##### EX-1
```c
#include <stdio.h>
int main(){
  
int day = 0;
printf("Enter a number between (1-7) :");
scanf("%d",&day);

switch (day){
    case 1:
        printf("Saturday");
        break;
    case 2:
        printf("Sunday");
        break;
    case 3:
        printf("Monday");
        break;
    case 4:
        printf("Tuesday");
        break;
    case 5:
        printf("Wednesday");
        break;
    case 6:
        printf("Thursday");
        break;
    case 7:
        printf("friday");
        break;
    default:
    printf("wrong input please enter between(1-7)");
}
return 0;
}
```