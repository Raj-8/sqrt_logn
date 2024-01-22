# sqrt_logn


int my_sqrt(int a)
{
    int l=0,r=5000000001;
    while(r-l>1)
    {
        int mid=(l+r)/2;
        if(1ll*mid*mid<=a)l=mid;
        else r=mid;
    }
    return l;
}
