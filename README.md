# landscapingclass Plant:
    def __init__(self, sunlight, water):
        self.sunlight = sunlight
        self.water = water
        self.energy = 0
    
    def photosynthesis(self):
        if self.sunlight > 0 and self.water > 0:
            self.energy += self.sunlight + self.water
            self.sunlight -= 1
            self.water -= 1
            print("Photosynthesis in progress...")
            print(f"Energy produced: {self.energy}")
        else:
            print("Insufficient sunlight or water for photosynthesis.")

# Creating an instance of a plant
plant = Plant(sunlight=5, water=3)

# Performing photosynthesis
plant.photosynthesis()
plant.photosynthesis()
plant.photosynthesis()
