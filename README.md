- 👋 Hi, I’m @Wasim-Akram1
- 👀 I’m interested in Coding and Playing Cricket  
- 🌱 I’m currently learning Data Structure 
- 💞️ I’m looking to collaborate on on open source projects that use Python C and C++
- 📫 How to reach me (wasimakramk60@gmail.com)

- #include<stdio.h>
#include<stdlib.h>
#include<time.h>
int main(){
    int number,guess,nguess=1;
    srand(time(0));
    number=rand()%100+1;
    //printf("The number is %d\n",number);
    do{
        printf("Guess the number between 1 to 100\n");
        scanf("%d",&guess);
        if(guess>number){
            printf("Lower Number Please\n");
        }
        else if(guess<number){
            printf("Higher Number Please\n");
        }
        else{
            printf("You Guessed it in %d attempts\n",nguess);
        }
        nguess++;
    }while(guess!=number);
    return 0;
}
