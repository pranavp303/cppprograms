#include <iostream>

using namespace std;

class EMI
{
    public:
    long long amount,interest;
    int rate,t;
    void getdata()
    {
        cout<<"Enter loan details"<<endl;
        cout<<"Enter Amount"<<endl;
        cin>>amount;
        cout<<"Enter Rate"<<endl;
        cin>>rate;
        cout<<"Enter Period"<<endl;
        cin>>t;
    }
    void installment()
    {
        int flag = 0;
        try
        {
            if(amount<50000)
            {
                throw 'a';
            }
            else if(amount>1000000)
            {
                throw 1;
            }
        }
        catch(char m)
        {
            cout<<"Error: Amount should not be less than 50000"<<endl;
            flag=1;
        }
        catch(int m)
        {
            cout<<"Error: Amount should not be more than 1000000"<<endl;
            flag=1;
        }
        try
        {
            if(rate<2)
            {
                throw 'a';
            }
            else if(rate>20)
            {
                throw 1;
            }
        }
        catch(char m)
        {
            cout<<"Error: Rate should not be less than 2"<<endl;
            flag=1;
        }
        catch(int m)
        {
            cout<<"Error: Rate should not be more than 20"<<endl;
            flag=1;
        }
        if(!flag)
        {
            long long inst,inst1;
            inst1=(amount * rate * t)/(100);
            inst=(inst1+amount)/(t*12);
            cout<<"Monthly installments will be "<<inst<<endl;
        }
    }
};

int main()
{
    EMI e1;
    e1.getdata();
    e1.installment();
    return 0;
}
