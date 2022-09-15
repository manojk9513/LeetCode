//balanced brackets using stack

#include <iostream>
#include <stack>

using namespace std;

bool balanceBracket(string exp){
    stack<char> sexp;

    for(int i=0;i<exp.length();i++){
        if(sexp.empty()){
            sexp.push(exp[i]);
        }
        else if((sexp.top()=='(' && exp[i]==')')||(sexp.top()=='{' && exp[i]=='}')||(sexp.top()=='[' && exp[i]==']'))
        {
            sexp.pop();
        }
        else{
            sexp.push(exp[i]);
        }
    }

    if(sexp.empty())return 1;
    return 0;
}

int main(){

    string str="{{}}[";

    if(balanceBracket(str))cout<<"Balanced";
    else cout<<"Not Balanced";
}
