# Importing all necessary  libraries
from pyowm import OWM
from pyowm.utils import config
from pyowm.utils import timestamps

# Setting up API key
owm = OWM ('e2fba7e993760e3851e3e7fa802f24ba') # valid API key

# Search for current weather in location (nearby city)
place = input("Enter Location: ")
mgr = owm.weather_manager()
observation = mgr.weather_at_place(place)
w = observation.weather

# Weather details
t = w.temperature("celsius")
t1 = t["temp"]
t2 = t["feels_like"]
t3 = t["temp_max"]
t4 = t["temp_min"]

# Output 
print(f"In the city of {place} temperature is now {t1}(°C), feels like {t2}(°C), maximum is {t3}(°C), minimum is {t4}(°C).")
