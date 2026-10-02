# Day-37-
My c language daily practice 
#include <iostream>
using namespace std;

int main()
{
    int a[5] = {50, 20, 40, 10, 30};

    for(int i = 0; i < 5 - 1; i++)
    {
        for(int j = 0; j < 5 - 1 - i; j++)
        {
            if(a[j] > a[j + 1])
            {
                int temp = a[j];
                a[j] = a[j + 1];
                a[j + 1] = temp;
            }
        }
    }

    cout << "Sorted array: ";

    for(int i = 0; i < 5; i++)
    {
        cout << a[i] << " ";
    }

    return 0;
}
