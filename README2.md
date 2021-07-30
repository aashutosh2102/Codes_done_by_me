## C Programs (Beginner level)
- Write a C Program to print your name.
```
#include <stdio.h>

int main() {
	printf("XYZ ABC");
	return 0;
}
```
- - Output
```
XYZ ABC
```

- Write a C Program to calculate sum of two numbers
```
#include <stdio.h>

int main() {
	int a=5, b=7, sum;
	sum=a+b;
	printf("%d",sum);
	return 0;
}
```
###### Run-time initallisation
```
#include <stdio.h>

int main() {
	int a,b,sum;
	printf("Enter the values of a & b\n");
	scanf("%d %d",&a,&b);
	printf("%d %d",a,b);
	sum=a+b;
	printf("\n%d",sum);
	return 0;
}
```
- - Outputs
```
12
```
###### Run-time initallisation
```
Enter the values of a & b
5 7
12
```

- Write a program to calculate Area of Circle.(Run-time)
```
#include <stdio.h>

int main() {
	float a, Area;
	printf("Enter the values of radius\n");
	scanf("%f",&a);
	int aa=a;
	printf("%d",aa);
	Area=(22/7)*a*a;
	printf("\n%f",Area);
	return 0;
}
```
- - Outputs
```
Enter the values of radius
5
75.000000
```
