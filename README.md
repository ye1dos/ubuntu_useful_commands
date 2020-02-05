# ubuntu_useful_commands


string isPossible2(int a, int b, int c, int d){
        if(b != d && b < d){
        b = b + a;}
        else if(a != c && a < c){
            a = a + b;
    }
    return isPossible2(a,b,c,d);
    }    
string isPossible(int a, int b, int c, int d){
    if(a == c && b == d){return "Yes";}
     else if(a != c && a < c){
        a = a + b;
    }
    else if(b != d && b < d){
        b = b + a;}
    else if(a != c && b != d){
        return "No";
    }
    else {
        return isPossible(b,a,c,d);}

    return isPossible(a,b,c,d);

    }
