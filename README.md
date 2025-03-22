``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## We live in a society bloated with data yet starved for wisdom. We're connected 24/7, yet anxiety, fear, depression and loneliness are at an all-time high. We must course-correct. - Elizabeth Kapu'uwailani Lindsey
