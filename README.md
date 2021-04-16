# Problem-1-Rectangle-Area-https-www.cs.scranton.edu-mccloske-hs_prog_contest-contest_problems-pro

#include<stdio.h>
#include<math.h>

typedef struct{
float x;
float y;
}point;

int main()
{
int n;
point P1,P2,P3;
float d1,d2;
float res[100];
printf("enter number of rectangle's area to be calculated");
scanf("%d",&n);
for(int i = 0;i < n ;i++)
{
printf("Enter three set of points");
scanf("%f%f%f%f%f%f",&P1.x,&P1.y,&P2.x,&P2.y,&P3.x,&P3.y);

d1 = sqrt ( pow((P1.x - P2.x),2) + pow((P1.y - P2.y),2));
d2 = sqrt ( pow((P1.x - P3.x),2) + pow((P1.y - P3.y),2));

float result = d1 * d2;
res[i] = result;
}

for(int j = 0;j<n;j++)
{
printf("Area of rectangle with vertices (%f,%f), (%f,%f) and (%f,%f) is %f\n",P1.x,P1.y,P2.x,P2.y,P3.x,P3.y,res[j]);

}
}
