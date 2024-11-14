# assignment-no.2.
name rahul lohiya 
aw-2

#include <stdio.h>
void menu();
void account1();
void account2();
void account3();
int submenu();
int Account1_Balance=0;
int Account2_Balance=0;
int Account3_Balance=0;

int main() {
   menu();
   
    return 0;
}
void menu(){
    int choice;
    printf("Press 1 to Choose Account 1:\nPress 2 to Choose Account 2:\nPress 3 to Choose Account 3:\n") ;
   
   printf("Enter the Choice from (1-3): ");
   scanf("%d",&choice);
   if(choice==1){
       account1();
   }else if(choice==2){
       account2();
   }else if(choice==3){
       //account3();
   }else{
       printf("Invalid Input!!");
   }

}
int submenu(){
    int choice;
    printf("Press 1 to Deposit\nPress 2 to Withdraw\nPress 3 to Check Balance:\n");
    printf("Enter the Choice from (1-3): ");
    scanf("%d",&choice);
    return choice;
}
void account1(){
int choice;
int deposit;
int withd;
int result=submenu();
    if(result==1){
        printf("Enter the Deposit Amount: ");
        scanf("%d",&deposit);
        if(deposit>0){
           Account1_Balance =Account1_Balance+deposit;
           printf("Amount Deposited successfully!!\n");
        }else{
            printf("Enter a valid Amount!!\n");
        }
    }else if(result==2){
        printf("Enter the Withdrawal Amount:");
        scanf("%d",&withd);
        if(withd>Account1_Balance){
            printf("Insufficient Amount!\n");
       }else{
           Account1_Balance=Account1_Balance-withd;
            printf("Amount Withdrawal successfully!!\n");
       }
    }else if(result==3){
          printf("Your Balance Amount: %d \n",Account1_Balance);
    }else{
          printf("Invalid Input!!\n");
         }
    printf("Press 1 For Main Menu\nPress any Key to Exit:\n");
    scanf("%d",&choice);
    if(choice==1){
        main();
    }else{
        printf("Program Exited Successfully!!\n");
    }
}
void account2(){
int choice;
int deposit;
int withd;
int result=submenu();
    if(result==1){
        printf("Enter the Deposit Amount: ");
        scanf("%d",&deposit);
        if(deposit>0){
           Account2_Balance =Account2_Balance+deposit;
           printf("Amount Deposited successfully!!\n");
        }else{
            printf("Enter a valid Amount!!\n");
        }
    }else if(result==2){
        printf("Enter the Withdrawal Amount:");
        scanf("%d",&withd);
        if(withd>Account2_Balance){
            printf("Insufficient Amount!\n");
       }else{
           Account2_Balance=Account2_Balance-withd;
            printf("Amount Withdrawal successfully!!\n");
       }
    }else if(result==3){
          printf("Your Balance Amount: %d \n",Account2_Balance);
    }else{
          printf("Invalid Input!!\n");
         }
    printf("Press 1 For Main Menu\nPress any Key to Exit:\n");
    scanf("%d",&choice);
    if(choice==1){
        main();
    }else{
        printf("Program Exited Successfully!!\n");
    }
}
void account3(){
int choice;
int deposit;
int withd;
int result=submenu();
    if(result==1){
        printf("Enter the Deposit Amount: ");
        scanf("%d",&deposit);
        if(deposit>0){
           Account3_Balance=Account3_Balance+deposit;
           printf("Amount Deposited successfully!!\n");
        }else{
            printf("Enter a valid Amount!!\n");
        }
    }else if(result==2){
        printf("Enter the Withdrawal Amount:");
        scanf("%d",&withd);
        if(withd>Account3_Balance){
            printf("Insufficient Amount!\n");
       }else{
           Account3_Balance=Account3_Balance-withd;
            printf("Amount Withdrawal successfully!!\n");
       }
    }else if(result==3){
          printf("Your Balance Amount: %d \n",Account3_Balance);
    }else{
          printf("Invalid Input!!\n");
         }
    printf("Press 1 For Main Menu\nPress any Key to Exit:\n");
    scanf("%d",&choice);
    if(choice==1){
        main();
    }else{
        printf("Program Exited Successfully!!\n");
    }
}
