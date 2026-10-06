# multilevel inheritance without constructor
class Shopping:
    def select_product(self):
        print("Customer selects a product")

class OnlineShopping(Shopping):
    def add_cart(self):
        print("Product added to cart")

class MobileShopping(OnlineShopping):
    def make_payment(self):
        print("Payment completed using mobile")

m = MobileShopping()
m.select_product()
m.add_cart()
m.make_payment()

# multilevel inheritance with constructor
class Company:
    def __init__(self, company_name):
        self.company_name = company_name

    def displaycompany(self):
        print("Company:", self.company_name)

class Employee(Company):
    def __init__(self, company_name, employee_name):
        super().__init__(company_name)
        self.employee_name = employee_name

    def displayemployee(self):
        super().displaycompany()
        print("Employee:", self.employee_name)

class Developer(Employee):
    def __init__(self, company_name, employee_name, language):
        super().__init__(company_name, employee_name)
        self.language = language

    def displaydeveloper(self):
        super().displayemployee()
        print("Language:", self.language)

d = Developer("Infosys", "Alekhya", "Python")
d.displaydeveloper()

# multilevel inheritance with constructor + super()
class Vehicle:
    def __init__(self, brand):
        self.brand = brand

    def displayvehicle(self):
        print("Brand:", self.brand)

class Car(Vehicle):
    def __init__(self, brand, model):
        super().__init__(brand)
        self.model = model

    def displaycar(self):
        super().displayvehicle()
        print("Model:", self.model)

class ElectricCar(Car):
    def __init__(self, brand, model, battery):
        super().__init__(brand, model)
        self.battery = battery

    def displayelectriccar(self):
        super().displaycar()
        print("Battery:", self.battery)
e = ElectricCar("Tesla", "Model 3", "75 kWh")
e.displayelectriccar()

# multilevel inheritance with constructor + super()

class Cricket:
    def __init__(self, player_name):
        self.player_name = player_name

    def displayplayer(self):
        print("Player Name:", self.player_name)

class Batsman(Cricket):
    def __init__(self, player_name, runs):
        super().__init__(player_name)
        self.runs = runs

    def displaybatsman(self):
        super().displayplayer()
        print("Runs:", self.runs)

class Captain(Batsman):
    def __init__(self, player_name, runs, team):
        super().__init__(player_name, runs)
        self.team = team

    def displaycaptain(self):
        super().displaybatsman()
        print("Team:", self.team)

c = Captain("Virat", 25000, "India")
c.displaycaptain()