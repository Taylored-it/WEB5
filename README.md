# WEB5
# Base class
class Superhero:
    def __init__(self, name, power, city):
        self.name = name
        self.power = power
        self.city = city

    def introduce(self):
        return f"I am {self.name} and I protect {self.city} with my {self.power}!"

    def use_power(self):
        return f"{self.name} uses {self.power}!"

# Subclass showing inheritance and encapsulation
class FlyingHero(Superhero):
    def __init__(self, name, power, city, altitude=0):
        super().__init__(name, power, city)
        self.__altitude = altitude  # private variable to show encapsulation

    def fly(self):
        self.__altitude += 1000
        return f"{self.name} is flying at {self.__altitude} feet!"

    def get_altitude(self):  # encapsulation via getter
        return self.__altitude
ASIIGNMENT 2
class Vehicle:
    def move(self):
        pass

class Car(Vehicle):
    def move(self):
        return "Driving on the road!"

class Plane(Vehicle):
    def move(self):
        return "Flying in the sky!"

class Boat(Vehicle):
    def move(self):
        return "Sailing on water!"
