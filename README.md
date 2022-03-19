#include"stdio.h"

int problem1(float a, float b){

  char virginica,versicolor,setosa;

  if(a<2.45 && !b<1.75)

   return setosa;

  else {

    if(b<1.75 && !a<4.95)

     return virginica;

    else {

     if(a<4.95 && !b<1.65)

      return virginica;

     else{

       if(b<1.65)

        return versicolor;

       else

        return virginica;
    }
   }
  }
 }

int problem2(float x, float y) {

  char virginica,versicolor,setosa;

  if(x<2.55 && !y<1.69)

   return setosa;

  else {

   if(y<1.69 && !x<4.85)

    return virginica;

   else {

    if(x<4.85)

     return versicolor;

    else

     return virginica;

   }
  }
 }

int main() {

  int problem;
  float PL,PW,SL,SW;
  float x1,x2,x3,x4,x5;

  printf("Select 1th, 2th or 3th problem: ");
  scanf("%d",&problem);

  if(problem==1) {

   printf("Enter PL:");
   scanf("%f",&PL);
   printf("Enter PW:");
   scanf("%f",&PW);
   printf("Enter SL:");
   scanf("%f",&SL);
   printf("Enter SW:");
   scanf("%f",&SW);

   char temp1=(char) problem1(PL,PW);
   char temp2=(char) problem2(PL,PW);

   if(temp1 == temp2) {

    printf("%s\n",temp1);
    printf("%s\n",temp2);
    printf("The first problem's answers are same\n");

     }

   else {

    printf("The first problem's answers are different");

    }
   }

  return 0;
}
