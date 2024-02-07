COWIN CHATBOT C++ Code
```
#include <iostream>
using namespace std;

int main()
{
    cout <<"WELCOME. What kind of enquiry do you have: \n1 = Medical \n2 = General \n3= Vaccine regiteration";
    int y;
    cout << "\nEnter a number: ";
    cin>> y;
    
    while(y>3)
    {
       cout <<"\nPlease enter a valid option.";
       cout <<"\nEnter a number:";
       cin>> y;
    }
    
    while(y==1)    //MEDICAL ENQUIRIES
    {
        cout << "\nWhat kind of medical enquiry: \n 1: Log symptoms \n 2: Medical support";
        int x;
        cout << "\nEnter a number:";
        cin >> x;
        
        while(x>2)  
        {
            cout <<"\nPlease enter a valid option.";
            cout <<"\nEnter a number:";
            cin >> x;
        }
        
        if(x==1)     //LOG SYMPTOMS
        {
            char s;
            cout << "\nPlease enter your symptoms: ";
            cin >> s;
            cout <<"\nWe will provide you with medical info on your specified symptoms shortly.";
        }
        else        //MEDICAL SUPPORT
        {
            cout << "\nFor medical support, contact '24754872984'.";
        }
        return 0;
    }
    
    while(y==2)        //GENERAL ENQUIRIES
    {
        cout<<"\nWhat is your general enquiry: \n 1: About the COWIN website \n 2: About COVID stats";
        int z;
        cout<<"\nEnter a number: ";
        cin >>z;
        
        while(z>2)
        {
            cout <<"\nPlease enter a valid option.";
            cout <<"\nEnter a number:";
            cin >> z;
        }
        
        if(z==1)      //ABOUT THE COWIN WEBSITE
        {
            cout<<"\nCoWIN is an Indian government web portal for COVID-19 vaccination registration, owned and operated by Indias Ministry of Health and Family Welfare. It displays booking slots of COVID-19 vaccine available in the nearby areas and can be booked on the website. For more information, please visit: 'https://www.cowin.gov.in/faq' ";
        }
        else          //ABOUT COVID STATS
        {
            cout<<"\nVisit:'https://www.mygov.in/covid-19'";
        }
        
        return 0;
    }
    
    while(y==3)       //VACCINATION REGISTERATION
    {
        int choice,t;    
        cout<<"\nAccording to your location, there are 4 available slots on the given date and time.\n 1)MGM Hospital \n2)Apollo Hospital \n3)Medicity \n4)UPHC2";
        cout<<"\nEnter your choice: ";
        cin >> choice;
        while(choice>4)
        {
            cout <<"\nPlease enter a valid option.";
            cout <<"\nEnter a number:";
            cin >> choice;
        }
        
        cout<<"Select time slot: ";
        cin>>t;
        switch(t)
        {
            case 1:
            cout<<"Time: 10:00AM-12:00PM";
            break;
            
            case 2:
            cout<<"Time: 12:00PM-2:00PM";
            break;
            
            case 3:
            cout<<"Time: 2:00PM-4:00PM";
            break;
            
            case 4:
            cout<<"Time: 4:00PM-6:00PM";
            break;
        }
        cout<<"\nThankyou. You have succefully registered for the vaccination. The slot ticket will be shared on your registered E-mail ID shortly.";
        return 0;
    }
    
    cout<<"\n\nTHANKYOU FOR VISITING COWIN CHATBOT.";
    return 0;
}
