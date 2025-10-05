import requests

# 🧭 Tutorial Mode
def run_tutorial():
    print("\n🧭 Tutorial Mode")
    print("Step 1: Choose your crop.")
    print("Step 2: Select soil and season.")
    print("Step 3: Simulate growth using satellite data.")
    print("Step 4: View dashboard to assess crop health.")

# 🌾 Crop Class
class Crop:
    def __init__(self, name, soil_type, season):
        self.name = name
        self.soil_type = soil_type
        self.season = season
        self.location = "Windhoek"
        self.health = 100

    def simulate_growth(self, climate):
        if climate['rainfall'] < 20:
            self.health -= 30
        elif climate['temperature'] > 35:
            self.health -= 20
        else:
            self.health += 10

# 🛰️ NASA POWER API Integration
def get_climate_data(location):
    latitude = -22.559
    longitude = 17.083
    url = f"https://power.larc.nasa.gov/api/temporal/daily/point?parameters=T2M,RH2M,PRECTOT&community=AG&longitude={longitude}&latitude={latitude}&format=JSON"
    response = requests.get(url)
    data = response.json()
    date_key = list(data['properties']['parameter']['T2M'].keys())[-1]
    return {
        "temperature": data['properties']['parameter']['T2M'][date_key],
        "humidity": data['properties']['parameter']['RH2M'][date_key],
        "rainfall": data['properties']['parameter']['PRECTOT'][date_key]
    }

# 📊 Dashboard
def show_dashboard(crop, climate):
    print("\n📊 AgriVerse Dashboard")
    print(f"Crop: {crop.name}")
    print(f"Soil Type: {crop.soil_type}")
    print(f"Season: {crop.season}")
    print(f"Health: {crop.health}")
    print("Climate Data:")
    print(f"  Temperature: {climate['temperature']} °C")
    print(f"  Humidity: {climate['humidity']} %")
    print(f"  Rainfall: {climate['rainfall']} mm")

# 🧠 Main Game Loop
def main():
    print("🌱 Welcome to AgriVerse 🌍")
    run_tutorial()

    crop = Crop("Maize", "Loamy", "Spring")
    climate = get_climate_data(crop.location)

    crop.simulate_growth(climate)
    show_dashboard(crop, climate)

if __name__ == "__main__":
    main()
