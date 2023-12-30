# online-ticket-booking-in-theatre
To book tickets in online mode, it consists of selecting movie, screen time and menu of snacks.
#include<stdio.h>
#define ROWS 10
#define COLS 10
void Recipt(char n[50],char g[50],char m[100]){
    printf("**The Recipt**\n");
    printf("Name:%s\n",n);
    printf("Gender:%s\n",g);
    printf("Movie Name:%s\n",m);
}
void bookTicket(int theater[ROWS][COLS], int row, int col) {
    if (row < 1 || row > ROWS || col < 1 || col > COLS) {
        printf("There is No Seat\n");
    }

    if (theater[row - 1][col - 1] == 0) {
        theater[row - 1][col - 1] = 1;
        printf("You have booked successfully for RowNo: %d, ColumnNo: %d.\n", row, col);
        printf("Your amount was Successfully paid\n");
    }
    else
    {
        printf("Seat in Row %d, Column %d is already booked. Please choose another seat.\n", row, col);
    }

}


int main(){
printf("Karur-1\n");
printf("Namakkal-2\n");
printf("Dindugal-3\n");
printf("Salem-4\n");
int place;
printf("Enter your Location from (1,2,3,4):\n");
scanf("%d",&place);
switch(place){
case 1:
    printf("Number of theatre:2\n");
    printf("The theatres are..,\n");
    printf("1-Ajantha\n");
    printf("2-Ellora\n");
    break;
case 2:
    printf("Number of theatre:3\n");
    printf("The theatres are..,\n");
    printf("1-Shiva\n");
    printf("2-Vikram Cinemas\n");
    printf("3-R S Theatre\n");
    break;
case 3:
    printf("Number of theatre:2\n");
    printf("The theatres are..,\n");
    printf("1-Carnival\n");
    printf("2-Rajendhra\n");
    break;
case 4:
    printf("Number of theatre:3\n");
    printf("The theatres are..,\n");
    printf("1-ARRS\n");
    printf("2-Ionix Cinemas\n");
    printf("3-KS Theatre\n");
    break;
default:
    printf("Invalid location Number\n");
    printf("Please choose from (1,2,3,4)\n");
    break;
}
printf("Choose a theatre:\n");
int theatre;
scanf("%d",&theatre);
switch(theatre){

case 1:
    if(place==1&&theatre==1){
    printf("The movies are:\n");
    printf("Joe->Rs.100\n");
    printf("*Siddha*Rs.150\n");
    printf("Number of screen:1\n");
    printf("The timings of the movies are..,:\n");
    printf("Joe-->10:00 AM - 1:00 PM && 7:00 PM - 10:00 PM\n");
    printf("Siddha-->2:00 PM - 5:00 PM\n");}
    else if(place==2&&theatre==1){
    printf("The movies are:\n");
    printf("Leo->Rs.200\n");
    printf("Jailer->Rs.150\n");
    printf("Annapoorni->Rs.100\n");
    printf("Japan->Rs.100\n");
    printf("Number of screen:2\n");
    printf("F.N:\n");
    printf("1st screen-->Leo && Timing-->10:00 AM - 1:00 PM \n");
    printf("2nd screen-->Jailer && Timing-->10:00 AM - 1:00 PM\n");
    printf("A.N:\n");
    printf("1st screen-->Annapoorni && Timing-->1:00 PM - 5:00 PM \n");
    printf("2nd screen-->Japan && Timing-->1:00 PM - 5:00 PM\n");}

    else if(place==3&&theatre==1){
    printf("The movies are:\n");
    printf("Kick->Rs.165\n");
    printf("Luck->Rs.100\n");
    printf("Joe->Rs.200\n");
    printf("Demon->Rs.170\n");
    printf("Number of screen:2\n");
    printf("F.N:\n");
    printf("1st screen-->Kick && Timing-->10:00 AM - 1:00 PM \n");
    printf("2nd screen-->Luck && Timing-->10:00 AM - 1:00 PM \n");
    printf("A.N:\n");
    printf("1st screen-->Joe && Timing-->1:00 PM - 5:00 PM \n");
    printf("2nd screen-->Demon && Timing-->1:00 PM - 5:00 PM\n ");}

    else{
    printf("The movies are:\n");
    printf("Japan->Rs.150\n");
    printf("Rangoli->Rs.100\n");
    printf("Number of screen:1\n");
    printf("The timings of the movies are..,:\n");
    printf("Japan-->10:00 AM - 1:00 PM && 7:00 PM - 10:00 PM\n");
    printf("Rangoli-->2:00 PM - 5:00 PM\n");
}
break;
case 2:
    if(place==1&&theatre==2){
    printf("The movies are:\n");
    printf("LGM->Rs.210\n");
    printf("Kolai->Rs.150\n");
    printf("ChandhraMugi-2->Rs.115\n");
    printf("Jawan->150\n");
    printf("Number of screen:2\n");
    printf("F.N:\n");
    printf("1st screen-->LGM && Timing-->10:00 AM - 1:00 PM \n");
    printf("2nd screen-->Kolai&& Timing-->10:00 AM - 1:00 PM\n");
    printf("A.N:\n");
    printf("1st screen-->ChandhraMugi-2 && Timing-->1:00 PM - 5:00 PM \n");
    printf("2nd screen-->Jawan && Timing-->1:00 PM - 5:00 PM\n");}
    else if(place==2&&theatre==2){
    printf("The movies are:\n");
    printf("Kick->Rs.175\n");
    printf("Luck->Rs.155\n");
    printf("Joe->Rs.200\n");
    printf("Iraivan->Rs.170\n");
    printf("Number of screen:2\n");
    printf("F.N:\n");
    printf("1st screen-->Kick && Timing-->10:00 AM - 1:00 PM \n");
    printf("2nd screen-->Luck && Timing-->10:00 AM - 1:00 PM\n");
    printf("A.N:\n");
    printf("1st screen-->Joe && Timing-->1:00 PM - 5:00 PM \n");
    printf("2nd screen-->Iraivan && Timing-->1:00 PM - 5:00 PM\n");}

    else if(place==3&&theatre==2){
    printf("The movies are:\n");
    printf("Leo->Rs.200\n");
    printf("Jailer->Rs.150\n");
    printf("Annapoorni->Rs.155\n");
    printf("Kick->Rs.175\n");
    printf("Number of screen:2\n");
    printf("F.N:\n");
    printf("1st screen-->Leo && Timing-->10:00 AM - 1:00 PM \n");
    printf("2nd screen-->Jailer && Timing-->10:00 AM - 1:00 PM \n");
    printf("A.N:\n");
    printf("1st screen-->Annapoorni && Timing-->1:00 PM - 5:00 PM \n");
    printf("2nd screen-->Kick && Timing-->1:00 PM - 5:00 PM\n ");}

    else{
    printf("Joe->Rs.180\n");
    printf("Siddha->Rs.155\n");
    printf("Number of screen:1\n");
    printf("The timings of the movies are..,:\n");
    printf("Joe-->10:00 AM - 1:00 PM && 7:00 PM - 10:00 PM\n");
    printf("Siddha-->2:00 PM - 5:00 PM\n");}
    break;
case 3:
    if(place==2 && theatre==3){
    printf("The movies are:\n");
    printf("NUN->Rs.170\n");
    printf("OMG->Rs.155\n");
    printf("Number of screen:1\n");
    printf("The timings of the movies are..,:\n");
    printf("The NUN-->10:00 AM - 1:00 PM && 7:00 PM - 10:00 PM\n");
    printf("Oh my God!-->2:00 PM - 5:00 PM\n");

}  else {
    printf("The movies are:\n");
    printf("Don->Rs.200\n");
    printf("Jawan->Rs.150\n");
    printf("OMG->Rs.200\n");
    printf("Nanban->Rs.155\n");
    printf("Number of screen:2\n");
    printf("F.N:\n");
    printf("1st screen-->Don && Timing-->10:00 AM - 1:00 PM \n");
    printf("2nd screen-->Jawan && Timing-->10:00 AM - 1:00 PM \n");
    printf("A.N:\n");
    printf("1st screen-->Oh my God! && Timing-->1:00 PM - 5:00 PM \n");
    printf("2nd screen-->Nanban && Timing-->1:00 PM - 5:00 PM\n ");}
    break;
default:
    printf("Invalid Theatre Number\n");
    printf("Please choose from availability of theatre\n");
    break;
}
      int theater[ROWS][COLS] = {0};
      int choice, row, col;


do
{
        printf("1. Book Ticket\n");
        printf("2. Exit\n");
        printf("Enter your choice: ");
        scanf("%d", &choice);
        char name[50];
        char gender[50];
        char movie[100];
        switch (choice)
        {

          case 1:
                printf("Enter your Name:\n");
                scanf("%s",name);
                printf("Enter your Gender:\n");
                scanf("%s",gender);
                printf("Select your movie:\n");
                scanf("%s",movie);
                printf("Enter the row and column to book a ticket : ");
                scanf("%d %d", &row, &col);
                Recipt(name,gender,movie);
                bookTicket(theater, row, col);
                break;

          case 2:
                printf("THANK YOU!\n");
                break;
 default:
                printf("Invalid choice\n");
        }
        break;
    } while(choice != 2);

printf("If you want to oder some snacks?\n");
printf("Yes-1 or No-2\n");
int Yn,Totalamt=0;
scanf("%d",&Yn);
if(Yn==1){
    printf("Snacks Menu:\n");
    printf("1. Popcorn - Rs.40\n");
    printf("2. Coffee - Rs.30\n");
    printf("3. Icecream - Rs.45\n");
    printf("4. Puffs - Rs.20\n");}
int Snacks[4]={1,2,3,4};
int count;
printf("Enter the count of Snacks:");
scanf("%d",&count);
for(int i=0;i<count;i++){
      printf("\nEnter your Snacks Number: ");
        scanf("%d", &Snacks[i]);

         if(Snacks[i]==1){
            Totalamt+=40;
        }
        else if(Snacks[i]==2){
            Totalamt+=30;
        }
        else if(Snacks[i]==3){
            Totalamt+=45;
        }
        else if(Snacks[i]==4){
            Totalamt+=20;
        }
        else {
           printf("Opps..! sry we dont have that Snacks in our Menu\n");
        }
}
   printf("Total amount of the snacks==>%d\n",Totalamt);
   printf("Thank you for your order. Enjoy the movie!\n");

}
