``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## What is new in the world? Nothing. What is old in the world? Nothing. Everything has always been and will always be. - Sai Baba
