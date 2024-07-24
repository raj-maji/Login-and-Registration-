# Login-and-Registration-


#include<iostream>

#include<vector>

using namespace std;

class user{

              private:

                           string username,password;

              public:

                           user(string name,string pass){

                                         username=name;

                                         password=pass;

                                        

                           }

             

};

class usermanager{

              private:

                           vector<user> users;

              public:

                           void regiseruser(){

                                         string username,password;

                                         cout<< "\t\t enter the name : ";

                                         cin>> username;

                                         cout<< "\t\t enter the password : ";

                                         cin>>password;

                                        

                                         user newuser(username,password);

                                         users.push_back(newuser);

                                        

                                         cout<<"\t\t user register successfully.......";

                                        

                           }

             

};

main(){

              usermanager usermanage;

             

              int op;

              cout<<"\t\t1 register user";

              cout<<"\t\t2 enter the choice : ";

              cin>>op;

              switch(op){

                           case 1:

                                         usermanage.regiseruser();

                                         break;

              }

}

