#  Single inheritance with polymorphism:
# Example 1:
print("------Vehicle-Bike-----------")
class Vehicle:
    def start(self):
        print("Vehicle starts")
class Bike(Vehicle):
    def start(self):
        print("Bike starts with a self-start")
v=Vehicle()
v.start()

b=Bike()
b.start()

# single Inheritance with polymorphism.
# Example 2:
print("-----Shape-Circle--------")
class Shape:
    def draw(self):
        print("Drawing a shape")
class Circle(Shape):
    def draw(self):
        print("Drawing a Circle")
s=Shape()
s.draw()

c=Circle()
c.draw()


# Multi Level Inheritance with Polymorphism.
# Example 3:
print("-------LivingThing-Animal-Bird---------")
class LivingThing:
    def action(self):
        print("Living thing Performs an action")
class Animal(LivingThing):
    def action(self):
        print("Animal eats")
class Bird(Animal):
    def action(self):
        print("Bird is flying")

livingthing=LivingThing()
livingthing.action()

animal=Animal()
animal.action()

bird=Bird()
bird.action()


# Multi Level Inheritance with Polymorphism.
# Example 2:
print("---------Device-Computer-Laptop------------")
class Device:
    def operator(self):
        print("Device is operating")
class Computer(Device):
    def operator(self):
        print("Computer is processing Data")
class Laptop(Computer):
    def operator(self):
        print("Laptop is running application")

device=Device()
device.operator()

computer=Computer()
computer.operator()

laptop=Laptop()
laptop.operator()


# Hierarichal inheritance with Polymorphism:
# Example 5:
print("------------Notification-Email&SMS--------")
class Notification:
    def send(self):
        print("Sending Notification")
class Email(Notification):
    def send(self):
        print("Sending notification through Email")
class SMS(Notification):
    def send(self):
        print("Sending notification through SMS")

email=Email()
email.send()

sms=SMS()
sms.send()


# Hierarichal inheritance with Polymorphism:
# Example 6:
print("------------Payment-UPIandCard--------------")
class Payment:
    def pay(self):
        print("Making Payment")
class UPI(Payment):
    def pay(self):
        print("Payment made using UPI")
class Card(Payment):
    def pay(self):
        print("Payment made using Card")

u=UPI()
u.pay()

c=Card()
c.pay()


# Multiple Inheritance with Polymorphism.
# Example 7:
print("------------Printer+Scanner-MultifunctionMachine------------")
class Printer:
    def operate(self):
        print("Printer prints documents")
class Scanner:
    def operate(self):
        print("Scanner scans documents")
class MultiFunctionMachine(Printer, Scanner):
    def operate(self):
        print("Machine prints and scans documents")


p=Printer()
p.operate()

s=Scanner()
s.operate()

m= MultiFunctionMachine()
m.operate()

# Multiple Inheritance with polymorphism.
# Example 8:
print("-------Telivison+InternetDevice-SmartTV-----------")
class Television:
    def operate(self):
        print("Television Displays channels")
class InternetDevice:
    def operate(self):
        print("Internet device connect to the internet")
class SmartTv(Television,InternetDevice):
    def operate(self):
        print("SmartTv displays channels and streams online content")
t=Television()
t.operate()

i=InternetDevice()
i.operate()

s=SmartTv()
s.operate()


# Hybrid Inheritance with polymorphism.
# Example 9:
print("-----person-student/Employee-intern------------")
class Person:
    def role(self):
        print("Person as a role")
class student(Person):
    def role(self):
        print("Student studies")
class Employee(Person):
    def role(self):
        print("Employee works")
class intern(student,Employee):
    pass

s=student()
s.role()

e=Employee()
e.role()

i=intern()
i.role()

# Hybrid Inheritance with polymorphism.
# Example 10:
print("---------Food-Vegetarian/Non-Vegetarian-Restaurant---------")
class Food:
    def prepare(self):
        print("Food is being prepared")
class Vegetarian(Food):
    def prepare(self):
        print("Preaparing Vegetarian Food")
class NonVegetarian(Food):
    def prepare(self):
        print("preparing NonVegetarian Food")
class Restaurant(Vegetarian,NonVegetarian):
    pass

v=Vegetarian()
v.prepare()

n=NonVegetarian()
n.prepare()

r=Restaurant()
r.prepare()