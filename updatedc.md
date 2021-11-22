#include<stdio.h>
#include<conio.h>
int not =0,noc=0,nor=0,nob=0,noeb=0,noec=0,amount=0,count=0;
// not == number of bus/truck
void truck()
{
  printf("ENTRY SUCESSFUL");
  not++;
  amount=amount+200;
  count++;
}
void car()
{
  printf("ENTRY SUCESSFUL");
  noc++;
  amount=amount+100;
  count++;
}
void rikshaw()
{
  printf("ENTRY SUCESSFUL");
  nor++;
  amount=amount+70;
  count++;
}
void bike()
{
  printf("ENTRY SUCESSFUL");
  nob++;
  amount=amount+50;
  count++;
}
void electricbike()
{
  printf("ENTRY SUCESSFUL");
  noeb++;
  amount=amount+90;
  count++;
}
void electriccar()
{
  printf("ENTRY SUCESSFUL");
  noec++;
  amount=amount+200;
  count++;
}
void status ()
{
printf("\nNumber of Bus/Truck=%d", not); 
printf("\nNumber of car/Jeep=%d", noc);
printf("\nNumber of rikshaw=%d", nor); 
printf("\nNumber of bike=%d", nob);
printf("\nNumber of electric bike=%d",noeb);
printf("\nNumber of electric car=%d", noec);
printf("\nTotal number of vehicles=%d", count);
printf("\nTotal amount=%d", amount);
}
void clear()
{
not=0;
noc=0;
nor=0;
nob=0;
noeb=0;
noec=0;
amount=0;
count=0;
printf("\nData cleared successfully");
}

int menu ()
{
int ch;
printf("\n\n\n 1. Enter bus/truck"); 
printf("\n 2. Enter car/jeep");
printf("\n 3. Enter rikshaw");
printf("\n 4. Enter  bike");
printf("\n 5. Enter Electric bike");
printf("\n 6. Enter Electric car");
printf("\n 7. check status");
printf("\n 8. clear data");
printf("\n 9 . exit");
printf("\n Enter your choice: ");
scanf("%d", &ch);
return (ch);
}
void main ( )
{
      while (1)
      {
         switch ( menu ( ))
{
 case1:
truck ( );
break;
case2:
car( );
break;
case3:
rikshaw( );
break;
case4:
bike ( );
case5:
electricbike();
 break;
case6:
electriccar();
break;
case7:
status();
 break;
case8:
clear();
 break;
case9:
 exit (0);
defalt:
printf("\n Enter correct option");
}
}
getch ();

}




























