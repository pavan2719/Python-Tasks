class Person:
    name="Ram"
    def walk():
        print(Person.name,"can Walk")
Person.walk()

class Human:
    age=20
    def vote():
        print("Eligible" if Human.age > 18 else "Not Eligible")
Human.vote()

class Even:
    n=6
    def checknum():
        print("Even" if Even.n%2==0 else "Odd")
Even.checknum()

class Greater:
    def checkGrater():
        print("15 is Greater" if 15 > 7 else "7 is Greater")
Greater.checkGrater()

class Part:
    def Hand():
        print("Every Human can Eat with their Hand")
Part.Hand()