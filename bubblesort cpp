#include <iostream>
int list[]={1,22,3,4,99,203,8,1,283,82,99,6,7,8,0};
int sizeoflist=sizeof(list)/sizeof(int);
bool issorted(int list[])
{
    bool issort;
    int n=0;
    for(int i=0;i<sizeoflist;i++)
    {
        if(i!=0)
        {
            if(list[i-1]>list[i])
            {
                issort=false;
                n+=1;
            }
        }
        if(n==0)
        {
            issort=true;
        }
    }
    return issort;
}

void sortlist(int list[])
{
    int buffer1,buffer2, buffer3;
    while(!issorted(list))
    {
        for(int i=0;i<sizeoflist;i++)
        {
            if(i!=0)
            {
                if(list[i-1]>list[i])
                {
                    buffer1=list[i-1];
                    list[i-1]=list[i];
                    list[i]=buffer1;
                }
            }   
        }
    }
}

int main() {
     for(int i=0;i<sizeoflist;i++){
        std::cout<<list[i]<<"-";}
        std::cout<<std::endl;
    
    sortlist(list);
    for(int i=0;i<sizeoflist;i++){
        std::cout<<list[i]<<"-";}
        std::cout<<std::endl;
        
    return 0;
}
