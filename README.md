``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Simply put, you believer that things or people make you unhappy, but this is not accurate. You make yourself unhappy. - Wayne Dyer
