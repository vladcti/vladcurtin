title: "Before/After Examples: Weather App Enhancements"
author: "vinesh dwarka davay"
format:
pdf:
toc: false
colorlinks: true
docx:
toc: false
highlight-style: github
html:
toc: true
toc-expand: 2
embed-resources: true

Example 1: Error Handling and Defaults

Initial Prompt

Can you help me write a weather app in Python that shows the temperature in a city?

Initial AI-Generated Code (Before)

import requests

city = "Perth"
response = requests.get(f"https://api.weatherapi.com/v1/current.json?key=KEY&q={city}")
data = response.json()
print(data["current"]["temp_c"])

My Analysis

Assumes city is always valid and API will succeed

No error handling or timeout

Hardcoded API key and city

Only prints temperature with no context

Follow-up Prompt

Can you improve this so it has error handling, uses a variable for the city, and shows both temperature and condition with labels? Also add a timeout.

Improved Code (After)

import requests

def get_weather(city):
    try:
        url = f"https://api.weatherapi.com/v1/current.json?key=KEY&q={city}"
        response = requests.get(url, timeout=5)
        response.raise_for_status()
        data = response.json()

        temp = data["current"]["temp_c"]
        condition = data["current"]["condition"]["text"]

        print(f"🌡️ Temperature in {city}: {temp}°C")
        print(f"☁️ Condition: {condition}")
    except Exception as e:
        print(f"⚠️ Could not retrieve weather data: {e}")

Why the Prompt Worked

Requested specific improvements (error handling, labels, flexibility)

AI followed up with helpful and structured output
