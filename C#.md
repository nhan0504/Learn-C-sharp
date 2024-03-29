# Comment
``` C#
// On line comment
/*
Multi line
*/
```
# Print out
``` C#
Console.Write("Hello World")
Console.WriteLine("Hello World")
```
# Variable
``` C#
string name = "Nhan";
Console.WriteLine("Hello " + name);

int num = 0;
```

# Data types
## Text
- String
``` C#
string name = "Nhan";
// Get the first character
Console.WriteLine(name[0])
// Get length of the string
Console.WriteLine(name.Length)
```
- Character
``` C#
char grade = "A";
```
## Number
``` C#
int age = 19;
// For decimal number from least precise to most precise
float, double, decimal
```
## Boolean
``` C#
bool isEmpty = true;
```

# Input
``` C#
string name =  Console.ReadLine();
// Get a number
int num = Convert.ToInt32(Console.ReadLine());
```

# Array
``` C#
// Need to specify the array size when create a new array
string[] strArray = new string[10];
int[] array = { 1, 2, 3};
```
## 2d Array
``` C#
int[,] matrix = new int[2,3];
int[,] number = {
    {1, 2},
    {2, 3},
    {3, 4 }
}

Console.Write(number[0, 0])
```

# Condition statement
``` C#
if (...) {...}
else {...}

switch (num) {
    case 1:
        ...
        break;
    case 2:
        ...
        break;
}
```

# Looping 
## While loop
``` C#
int i = 0;
while (i < 5) {
    Console.WriteLine(i);
    i++;
}
```
## For loop
``` C#
for (int i = 0; i < 5, i++) {
    Console.WriteLine(i);
}
```

# Error handling
``` C#
try {...}
catch(Exception e) {
    Console.WriteLine(e.Message);
}
// Catch multiple specific error
try {...}
catch(FormatException e) {
    Console.WriteLine(e.Message);
}
catch(NullReferenceException e) {
    Console.WriteLine(e.Message);
}
```

# Object and class
``` C#
class Student {
    public string name;
    private int gpa;
}

Student myStudent = new Student();
```
## Constructor
``` C#
class Student {
    public string name;
    private int gpa;
}

public Student(string name, int gpa) {
    name = name;
    gpa = gpa;
}
```

## Method
``` C#
class Student {
    public string name;
    private int gpa;
}

public boolean isHonor() {
    if (gpa > 3.5) {
        return true;
    }
    return false;
}
```

## Getter and setter
``` C#
class Student {
    public string name;
    private int gpa;
}

public Student(string name, int gpa) {
    name = name;
    // Use the Rating setter method
    Gpa = gpa;
}

public string Gpa {
    get { return gpa; }
    set {
        if (gpa <=0 || value > 4) {
            gpa = null;
        } else {
            gpa = value;
        }
    }
}
```

# Inheritance
- Inherit a class
``` C#
class Animal {
    ...
}

// Class Dog inherit class Animal
class Dog: Animal {

}
```
- Overwrite a method in the superclass. Have to specify that method in the superclass as virtual -> Allow subclass to overwrite
``` C#
class Animal {
    public virtual void eat() {
        ...
    }
}

class Dog: Animal {
    public override void eat() {
        ...
    }
}
```