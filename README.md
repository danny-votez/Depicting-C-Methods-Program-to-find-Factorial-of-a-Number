# Depicting-C-Methods-Program-to-find-Factorial-of-a-Number
// This program is aimed at depicting C++ Methods
// To do this, there is using an example of a program that calculates factorial of a number
// That is, with factorial, the operation is: n! = n*(n-1)*(n-2)*(n-3)........4*3*2*1

#include<iostream>
using namespace std;
class Method{
    private: int Number;
    public: void Get(){
        cout<<"Enter a number you wish to find its Factorial: "<<endl;
        cin>>Number;
        cout<<"The result of "<<Number<<"! is: "<<Factor(Number);   /// Initiate a call
    }
    public: int Factor(int N){
        if (N == 0){            // This forms teh base condition
            return 1;
        }
        else{
            return N*Factor(N-1);     /// This is for example, 5!  = 5*4*3*3*1
        }
    }
};
int main(){
    Method M;
    M.Get();
    return 0;
}
