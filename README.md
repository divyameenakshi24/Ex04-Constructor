# Ex04-Constructor
## Aim:
 To write a C# program to calculate the salary of an employee by passing the name, designation, noofexperience, basic salary and insurance amount through constructor.
 
 ## Algorithm:
 ### Step1:
 
 
 
 ## Program:
 ```
 using System;
namespace Exception
{ 
    public class Employee
    { 
        public String work, name;
        public int exp,bs,insurance;
        double hra,ta,salary;
        public Employee(String name, String work, int exp, int bs, int insurance)
        {
            this.name = name;
            this.work = work;
            this.exp = exp;
            this.bs = bs;
            this.insurance = insurance;
        }
        public void Salary()
        {
            hra = this.bs * 0.2;
            ta = this.bs * 0.1;
            salary = this.bs + hra + ta-this.insurance;
        }
        public void display()
        {
            Console.WriteLine("Name of the employee is " + this.name + " having " + this.exp + " of experience, working as " + this.work + " Receives " + salary + " of salary");
        }
    }
    class TestEmployee
    {
        public static void Main(string[] args)
        {
            Employee e1 = new Employee("Hari", "Tester", 10, 30000, 1000);
            Employee e2 = new Employee("Latha", "Developer", 5, 25000, 1000);
            e1.Salary();
            e2.Salary();
            e1.display();
            e2.display();

        }
    }
}
```
 
 ## Output:
 ![Screenshot 2022-05-05 161611](https://user-images.githubusercontent.com/75235402/166908587-a7365e85-23ee-49d2-a503-6565d7f4b3f8.jpg)

 ## Result:
