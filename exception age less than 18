#include <iostream>
using namespace std;
int main() {
    string vote;
    int age, BJP = 0;
    int Congress = 0;
    cout << "Enter Age:";
    cin >> age;
    try{
        if(age <18){
            throw age;
        }
        else{
            cout << "You can vote\n "<<endl;
        }
    }
    catch(int age){
        cout << "\nYour age is "<<age<<" cannot vote.";
    }

    cout << "Whom you want to Vote?(BJP/Congress)";
    cin >> vote;
    if(age >=18){
    if(vote == "BJP"){
        BJP++;
        cout << "Thank you for Voting....";
    }
    else if(vote == "Congress"){
        Congress++;
        cout << "Thank you for Voting....";
    }
    else{
        cout << "Enter correctly";
    }
    }
    return 0;
}
