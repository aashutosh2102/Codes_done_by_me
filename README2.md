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

- Write a C program to calculate roots of a quadratic equations(For real roots)
###### Root(r1,r2) values as (+-b + sqrt(b*b-4ac))/2a
```
#include <stdio.h>
#include<math.h>
int main() {
	float a,b,c,r1,r2;
	printf("Enter the values of a,b,c");
	scanf("%f %f %f",&a,&b,&c);
	int aa=a,bb=b,cc=c;
	printf("\n%d %d %d",aa,bb,cc);
	r1=(-b+sqrt(pow(b,2)-4*a*c))/2*a;
	r2=(-b-sqrt(pow(b,2)-4*a*c))/2*a;
	printf("\nRoots are as %f and %f",r1,r2);
	return 0;
}
```
- - Output
```
Enter the values of a,b,c
1 2 1
Roots are as -1.000000 and -1.000000
```

- Write a C program to calculate semi-perimeter and Area of Triangle only using the sides values.
###### Apply Heron's Formula
```
#include <stdio.h>
#include<math.h>
int main() {
    float a,b,c,S,Area;
    printf("Enter the values of a,b,c");
    scanf("%f %f %f",&a,&b,&c);
    S=(a+b+c)/2;
    Area=sqrt(S*(S-a)*(S-b)*(S-c));
    int aa=a,bb=b,cc=c;
    printf("\n%d %d %d\n",aa,bb,cc);
    printf("Semi-Perimeter = %0.2f\nArea = %0.2f",S,Area);
	return 0;
}
```
- - Output
```
Enter the values of a,b,c
10 11 20
Semi-Perimeter = 20.50
Area = 31.98
```

- Write a C program to find out the total shopping amount of a person if he gets 50% discount on the total amount.(Run-time)
```
#include <stdio.h>
#include<math.h>
int main() {
    float Total_value,Discounted_value;
    printf("Enter the total value of shopping\n");
    scanf("%f",&Total_value);
    Discounted_value=Total_value/2;
    int tt=Total_value;
    printf("%d",tt);
    printf("\nDiscounted_value = %0.3f",Discounted_value);
	return 0;
}
```
- - Output
```
Enter the total value of shopping
10000
Discounted_value = 5000.000
```

- Write a C program to input marks obtained by a student in 5 subjects. Calculate the average marks and percentage obtained by the student.
```
#include <stdio.h>

int main() {
    float E,H,M,S,St,Av,P;
    printf("Enter the marks obtained in E,H,M,S,St in serial order.\n");
	scanf("%f %f %f %f %f",&E,&H,&M,&S,&St);
	Av=(E+H+M+S+St)/5;
	P=(E+H+M+S+St)/5;
	int e=E,h=H,m=M,s=S,sT=St;
	printf("%d %d %d %d %d",e,h,m,s,sT);
	printf("\nAverage marks = %f",Av);
	printf("\nPercentage obtained is %f",P);
	return 0;
}
```
- - Output
```
Enter the marks obtained in E,H,M,S,St in serial order.
89 92 100 100 75
Average marks = 91.199997
Percentage obtained is 91.199997
```
