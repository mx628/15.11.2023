#include <iostream>
#include <string>
using namespace std;
int strmax(string a, string b){
    int isnA = 0, isnB = 0;
    if(a[0] == '-')
        isnA = 1;
    if(b[0] == '-')
        isnB = 1;
    if(a.size() - isnA > b.size() - isnB)
        return a.size();
    if(a.size() - isnA < b.size() - isnB)
        return b.size();
    return a.size();
}
string rev(string str){
    string str2;
    int n = 0;
    if(str[0] == '-')
        n = 1;
    for(int i = n; i < (str.size()-n)/2 + n; i++){
        char tmp = str[i];
        str[i] = str[str.size() - i - 1 + n];
        str[str.size() - i - 1 + n] = tmp;
    }
    if()
    return str;
}
string oper(string a, string b, int op){ //0 - слож. 1 - выч. 2 - умн. 3 - дел.
    int isnegA = 1, isnegB = 1;
    string str;
    if(a[0] == '-')
        isnegA = -1;
    if(b[0] == '-')
        isnegB = -1;
    a = rev(a);
    b = rev(b);
    //-------------------------
    if(isnegB == 1 && isnegA == 1 && op == 0){
//        for(int i = 0; i < )
    }
}
int main()
{
    cout << rev("-123456789");
    return 0;
}
