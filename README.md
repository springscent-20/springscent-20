``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## The greatest danger for most of us is not that our aim is too high, and we miss it, but that it is too low, and we reach it. - Michelangelo
