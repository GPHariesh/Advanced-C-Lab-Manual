EXP NO:1 C PROGRAM FOR ARRAY OF STRUCTURE TO CHECK ELIGIBILITY FOR THE VACCINE.

Aim:
To write a C program for array of structure to check eligibility for the vaccine person age above 6 years of age.

Algorithm:
1.	Declare structure eligible with age (integer) and n (character array)
2.	Declare variable e of type eligible
3.	Input age and name using scanf, store in e
4.	If e.age <= 6
-	Print "Vaccine Eligibility: No"
Else
-	Print "Vaccine Eligibility: Yes"
5.	Print details (e.age, e.n)
6.	Return 0
 
Program:
```
#include <stdio.h>
struct exp{
    int age;
    char n[50];
};

int main() {
    struct exp e[3];
    int i;
    for(i=0;i<3;i++){
       
        scanf("%d",&e[i].age);
        scanf("%s",e[i].n);
    }
    for(i=0;i<3;i++){
        printf("Age: %d Name : %s\n",e[i].age,e[i].n);
        if(e[i].age<=6){
            printf("Vaccine Eligibility:No\n");
        }
        else{
             printf("Vaccine Eligibility:yes\n");
        }
        
    }
    
}
```


Output:
<img width="623" height="368" alt="image" src="https://github.com/user-attachments/assets/9322a814-fcc5-44c0-ac48-6fb9fd17c5a6" />


// paste the output screenshot


Result:
Thus, the program is verified successfully.
