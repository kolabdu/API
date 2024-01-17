# API
I was presented with an intriguing task—to fetch weather data from an API. Recalling my previous encounter with API interactions during my training at DataCamp, I realized that relying solely on `pd.read_csv()` didn't cover all the intricacies involved, and some aspects, like the concept of a base URL, slipped my mind.

Determined to overcome this challenge, I turned to YouTube for guidance. A specific video caught my attention and provided valuable insights, reorienting me on the right path. However, my progress hit a snag as the API key I had generated came with limitations.

Undeterred, my quest led me to another YouTube channel called "Growing Scientist," where I discovered a video titled "Download Historical Weather Data for Free Without Using API." This innovative approach proved to be the solution I needed, successfully completing the task at hand.

![Alt text](![Capture](https://github.com/kolabdu/API/assets/54320228/fa5098c6-bdf5-456f-89c8-d3493ccdda32)
)




my code

import requests

API_KEY = "fc179f8a20e64f8a883173714241001"
CITY = "Lagos"
BASE_URL = f"https://lnkd.in/dBKfcJFu"

response = requests.get(BASE_URL).json()

print(response)
