## C Programs (Beginner level)
##### IDE USED --> https://ide.geeksforgeeks.org/
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

- Write a C program to calculate SI and CI.
```
#include <stdio.h>
#include<math.h>
int main() {
	float SI,P,R,T,CI;
	printf("Enter the values of P, R, T\n");
	scanf("%f %f %f",&P,&R,&T);
	SI=(P*R*T)/100;
	CI=(P*pow(1+R/100,T)-P);
	int p=P,r=R,t=T;
	printf("%d %d %d",p,r,t);
	printf("\nSi is %f\nAnd, CI is %f",SI,CI);
	return 0;
}

```
- - Output
```
Enter the values of P, R, T
1000 2 3
Si is 60.000000
And, CI is 61.207939
```

- Write a C program to implement distance formula.
###### d=sqrt(pow((x2-x1),2)+pow((y2-y1),2))
```
#include <stdio.h>
#include<math.h>
int main() {
    float x1,x2,y1,y2,d;
    printf("Enter the coordinates as x1, x2, y1, y2\n");
    scanf("%f %f %f %f",&x1,&x2,&y1,&y2);
    int xx1=x1,yy1=y1,xx2=x2,yy2=y2;
    printf("%d %d %d %d",xx1,xx2,yy1,yy2);
    d=sqrt(pow((x2-x1),2)+ pow((y2-y1),2));
    printf("\nDistance is %f",d);
	return 0;
}
```
- - Output
```
Enter the coordinates as x1, x2, y1, y2
10 20 30 40
Distance is 14.142136
```
