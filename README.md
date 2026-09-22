#include <bits/stdc++.h>
using namespace std;
#define z endl
#define ll long long
#define f float

class Rectangle
{
public:
    int length, width;
    void compareArea(Rectangle r);
};
inline void Rectangle::compareArea(Rectangle r)
{
    int area1 = length * width;
    int area2 = r.length * r.width;
    if (area1 > area2)
        cout << "First area" << z;

    else if (area2 > area1)
        cout << "Second  area" << z;
    else
        cout << "Both equal area." << z;

}

int main()
{
    Rectangle s1, s2;
    s1.length = 10;
    s1.width = 5;
    s2.length = 8;
    s2.width = 4;

    s1.compareArea(s2);

    return 0;
}
