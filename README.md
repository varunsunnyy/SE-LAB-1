# SE-LAB-1
# SE LAB PROGRAMS

def calculate_Weather(T, H, w):
    W = 0.5 * (T**2) - 0.2 * H + 0.1 * w - 15
    return W

def classify_weather(W):
    if W > 300:
        return "Sunny"
    elif 200 < W <= 300:
        return "Cloudy"
    elif 100 < W <= 200:
        return "Rainy"
    elif W <= 100:
        return "Stormy"
    else:
        return "Undefined"  

T = int(input("Enter the value for T (temperature): "))
H = int(input("Enter the value for H (humidity): "))
w = int(input("Enter the value for w (wind speed): "))

result_W = calculate_Weather(T, H, w)
weather_condition = classify_weather(result_W)

print(f"The value of W is: {result_W}<br>")
print(f"The weather condition is: {weather_condition}<br>")
