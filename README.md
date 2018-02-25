# BCS230
C++
//Just for practice
#include <iostream>
#include<cmath>
#include <iomanip>
using namespace std;

class Surgery
{
  private:
    int type;
    double cost;
    
  public:
  
    void setType(int t)
    {
      type=t;
    }
    
    void setS_cost(int t,double cst)
    {
      cost=cst;
    }
    
   double getSurCost()
   {
      if(type==1)
       {cost=100.0;}
      else if(type==2)
        {cost=200.0;}
      else if(type==3)
        {cost=300.0;}
      else if(type==4)
        {cost=400.0;} 
      else if(type==5)
        {cost=500.0;}
     return cost;
   }
};
int main() {
  int t1=4;
  double cc;
  Surgery s1;
  s1.setS_cost(t1,cc);
  cout<<fixed<<showpoint<<setprecision(2)<<endl;
  cout<<s1.getSurCost()<<endl;;
  
  return 0;
}
