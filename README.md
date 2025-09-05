#include<iostream>
using namespace std;

class Point 
private:
int x;
int y;
char symbol;
public:
    void Print()
    {
        cout << symbol << "-> X: " << x << "\tY: " << y << endl;
    }
    void Init(char t, int _x, int _y)
    {
    symbol = t;
    x = _x;
    y = _y;
    }
void Sum(Point b)
{
    cout << "X: " << x + b.x << "\tY: " << y + b.y << endl;
}
void Min(Point b) {
    cout << "X: " << x - b.x << "\tY: " << y - b.y << endl;
}
void Mul(Point b) {
    cout << "X: " << x * b.x << "\tY: " << y * b.y << endl;
}
int main()
{
    Point a, b;

    a.Init('A', 10, -20);
    a.Print();

    b.Init('B', 5, 16);
    b.Print();

    a.Sum(b);
    a.Min(b);
    a.Mul(b);



}
