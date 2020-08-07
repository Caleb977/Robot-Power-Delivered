#include<stdio.h>
int main(){
    int NumberOfRobot;
    int EnginePower;
    int Resistance;
    int Weight;
    int Height;
    int TotalPower;
    int GeneralPower = 0;
    int i;
    
    printf("How many robots do you want to deploy:\n");
    scanf("%d",&NumberOfRobot);
    
    for(i=0; i<NumberOfRobot; i++){
        puts("EnginePower:");
        scanf("%d",&EnginePower);
        
        puts("Resistance rating (1,2, or 3 only):");
        scanf("%d",&Resistance);
        
        puts("Robot Weight. Note \"The Weight should be greater than the Height\":");
        scanf("%d",&Weight);
        
        puts("Robot Height:");
        scanf("%d",&Height);
        
        TotalPower = (EnginePower+Resistance)*(Weight-Height);
        printf("Power of Robot = %d\n",TotalPower);
        
        GeneralPower = GeneralPower + TotalPower; 
        printf("General Power delivered = %d\n", GeneralPower);
    }
 return 0;
    
}
