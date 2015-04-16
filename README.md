# quiz-9.3

#include <iostream>
using namespace std;

long fibonacci(int n){
int i = 2;
long x= 0, y = 1, z= 0;

if(n == 1){
i = n + 1;
}
else{
if(n == 2){
z = 1;
i = n + 1;
}
else{

do{
i = i + 1;
z = x + y;
x = y;
y = z;

}while(i<n);
}
}
return z;

}

int main(){
int n;
long u;
cout << "Posision de la serie de fibonacci a saber" << endl;
cin >> n;

u = fibonacci(n);

cout << "En el lugar " <<n<< " se encuentra el numero " << u<<endl;

return 0;

}
