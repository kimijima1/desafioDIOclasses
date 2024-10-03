class Hero:
    def __init__(self, name, age, hero_type):
        self.name = name
        self.age = age
        self.hero_type = hero_type

    def show_details(self):
        return f"Hero: {self.name}, Age: {self.age}, Type: {self.hero_type}"

    def attack(self):
        if self.hero_type.lower() == "mage":
            attack = "casted firebolt"
        elif self.hero_type.lower() == "warrior":
            attack = "struck with a sword"
        elif self.hero_type.lower() == "monk":
            attack = "dealt a flurry of blows"
        elif self.hero_type.lower() == "ninja":
            attack = "threw a shuriken"
        else:
            attack = "attacked with... something"

        print(f"The {self.hero_type} {attack}")

hero1 = Hero("Gandalf", 100, "mage")


hero1.attack()  
print(hero1.show_details())  
