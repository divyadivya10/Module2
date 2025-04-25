## 2A DYNAMIC MEMORY ALLOCATION

## PROGRAM STATEMENT:
 To Write A CPP Program to allocate memory dynamically for an long integer variable. (Note: p_var = new typename;)

 ## ALGORITHM:
1. Start the program.
2. Define a class var_space with a method allocateSpace that dynamically allocates memory for a
long integer, reads a value from the user, and prints it.
3. In the main function, create an object of var_space and call allocateSpace.
4. End the program

## PROGRAM:
```
#include<iostream>
using namespace std;
class var_space
{
    public:
    void allocatespace()
    {
        int *p_var= new int;
        cin>>*p_var;
        cout<<"Long Value is : "<<*p_var;
    }
};

int main()
{
    var_space s;
    s.allocatespace();
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/0dc6101f-b76e-4cd0-84af-3f474ce51a55)

## RESULT:
Thus, the C++ program to allocate memory dynamically for a long integer variable is created
successfully.

## 2B STATIC CLASS MEMBERS

## PROGRAM STATEMENT:

 To Write A CPP Program to create class RectangleBox and calculate the volume of the rectangleBoxe use of static member variable in the class RectangleBox.

## ALGORITHM:

1.Define a Box class with private variables for length, breadth, and height.
2.Use a static variable objcount to keep track of the number of Box objects created.
3.Implement a constructor that initializes the dimensions, prints a message, and increments objcount.
4.Create a Volume() function to return the calculated volume of the box.
5.In main(), create two Box objects, print their volumes, and display the total number of objects created.

## PROGRAM:
```
#include <iostream>
 
using namespace std;

class Box 
{
    public:
    static int objcount;
    Box(double l,double b,double h)
    {
        length=l;
        breadth=b;
        height=h;
        cout<<"Constructor called."<<endl;
        objcount++;
    }
    double Volume()
    {
        return length*breadth*height;
    }
    private:
    double length;
    double breadth;
    double height;
};
int Box::objcount=0;
int main(void)
{
    int l,b,h,l1,b1,h1;
    cin>>l>>b>>h>>l1>>b1>>h1;
    Box box1(l,b,h);
    cout<<"Volume :"<<box1.Volume()<<endl;
    Box box2(l1,b1,h1);
    cout<<"Volume :"<<box2.Volume()<<endl;
    cout<<"Total objects: "<<Box::objcount;
    return 0;
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/27e54c2b-b3dc-43e3-84fd-6971a5aed0c8)

## RESULT:  
Thus, a CPP Program to create class RectangleBox and calculate the volume of the rectangleBoxe use of static member variable in the class RectangleBox is created successfully

## FUNCTION OVERLOADING

## PROGRAM STATEMENT:
 
   To Write a CPP program to overload a function to print Integer data in one and Floating-Point data in another
  
## ALGORITHM:

1.Define a class function with two overloaded print functions: one for integers and one for floating-point numbers.
2.The first print function takes an integer as input and displays it with the label "Integer".
3.The second print function takes a floating-point number as input and displays it with the label "Floating Point".
4.In the main() function, create an object f of class function.
5.Take an integer and a float as input, and call the appropriate print function for each to display the values.

## PROGRAM:
```
#include<iostream>
using namespace std;
class function
{
    public:
    void print(int x)
    {
        cout<<"Integer="<<x<<endl;
    }
    void print(float x)
    {
        cout<<"Floating Point="<<x;
    }
};
int main()
{
    function f;
    int x;
    float y;
    cin>>x>>y;
    f.print(x);
    f.print(y);
    return 0;
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/9e0468bd-3dea-46bf-9861-47e8ca5162f6)


## RESULT:  
Thus, To Write a CPP program to overload a function to print Integer data in one and Floating-Point data in another is created successfully.

## OPERATOR OVERLOADING

## PROGRAM STATEMENT:

  To Write a CPP Program to overload the Operator (++) i.e. on invoking it the incrementation should happen by some random value.
  
## ALGORITHM:

1.Define a class count with three public variables: value, value1, and value2.
2.Overload the ++ operator to calculate the sum of value1 and value2 and assign it to value, then print value.
3.In the main() function, create an object c1 of the class count.
4.Take input values for value1 and value2 from the user.
5.Call the overloaded ++ operator on the object c1 to calculate and display the sum of value1 and value2.

## PROGRAM:
```
#include<iostream>
using namespace std;
class count
{
    public:
    int value,value1,value2;
    void operator ++()
    {
        value=value1+value2;
        cout<<value;
    }
};
int main()
{
    count c1;
    cin>>c1.value1>>c1.value2;
    ++c1;
    return 0;
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/1e77bbef-ae9e-4509-b123-996c0aa810e1)



## RESULT:  
Thus, To Write a CPP Program to overload the Operator (++) i.e. on invoking it the incrementation should happen by some random value. is created successfully.









