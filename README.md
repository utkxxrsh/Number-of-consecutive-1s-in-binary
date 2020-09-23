# Number-of-consecutive-1s-in-binary

 #include <iostream>  
 using namespace std;  
 int main(){  
      int n;  
      cin >> n;  
      int maxConsecutive, currentConsecutive = 0;  
      while (n > 0) {  
           if (n % 2 == 1){  
                currentConsecutive++;  
                if (currentConsecutive > maxConsecutive)  
                     maxConsecutive = currentConsecutive;  
           } else {  
                currentConsecutive = 0;  
           }  
           n /= 2;  
      }  
      cout << maxConsecutive;  
 }  
