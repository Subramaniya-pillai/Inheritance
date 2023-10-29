# EX08-Inheritance

## Aim:

To write a C# program to print some messages using hierarchical inheritance.

## Algorithm:

step 1: Create a base class.

Step 2: Create two child class.

step 3: Create a constructor in the base class and print a message.

step 4: Create a function in child class to print a message.

step 5: End the program.

## Program:
> Developed by : Subramaniya Pillai B

> Reg.no: 21222230109
```
using System;
public class tyre
{
/* public tyre()
{
Console.WriteLine("Give the tyre type: ");
}*/
public virtual void display()
{
Console.WriteLine("Give the tyre type: ");
Console.Write("Tyre type = ");
}
}

public class car : tyre
{
public override void display()
{
base.display();
Console.WriteLine("Car tyre");
}
}

public class scooter : tyre
{

public override void display()
{
base.display();
Console.WriteLine("Scooter tyre");
}
}
public class program
{
static void Main()
{
car c = new car();
c.display();
Console.WriteLine();
scooter s = new scooter();
s.display();
}
}
```

## Output:
![](./1.png)

## Result:
Thus C# program to print messages using hierarchical inheritance is written and executed sucessfully.
