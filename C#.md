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