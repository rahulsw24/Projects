#include <iostream>
#include <string.h>
using namespace std;
struct encryption
{
    char enc[200];
    char plaintext[200];
    char ciphertext[200];
    int key;
};
int main()
{
    struct encryption e;
    char username[20],password[20],uname[20]="p1",pass[20]="p2",ch;
    int op;
    cout<<"\n Security of your Information Matters \n";
    cout<<"---------------------------------------- \n";
    cout<<"Enter username : ";
    cin>>username;
    cout<<"Enter password : ";
    cin>>password;
    if(strcmp(username,uname)==0 && strcmp(password,pass)==0)
    {
        cout<<"Welcome to encryption world \n";
        do{
        cout<<"1. Encryption \n";
        cout<<"2. Decryption \n";
        cout<<"3. EXIT \n";
        cout<<"Enter your option";
        cin>>op;
            switch (op) {
                case 1:
                    cout<<"Enter Encryption key \n";
                    cin>>e.key;
                    fflush(stdin);
                    cout<<"Enter the plain text \n";
                    cin.get(e.plaintext,200);
                    cout<<"The cipher text is \n";
                    for(int i=0;i<strlen(e.plaintext);i++)
                    {
                    e.enc[i]=(int)e.plaintext[i]+e.key;
                        cout<<e.enc[i];
                    }
                    break;
                case 2:
                    cout<<"Enter Encryption key \n";
                    cin>>e.key;
                    fflush(stdin);
                    cout<<"Enter the text you want to decrypt \n";
                    cin.get(e.ciphertext,200);
                    cout<<"The plain text is \n";
                    for(int i=0;i<strlen(e.ciphertext);i++)
                    {
                        e.plaintext[i]=(int)e.ciphertext[i]-e.key;
                        cout<<e.plaintext[i];
                    }
                    break;
                case 3:
                    cout<<"This is the EXIT Case \n";
                    exit(0);
                default:
                    cout<<"Please enter the correct number";
            }
            cout<<" \n Do You want to continue \n";
            cout<<"For YES enter Y/y, for NO press any key \n";
            cin>>ch;
        }while (ch=='y'||ch=='Y');
}
    return 0;
}
