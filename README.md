``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## What makes Superman a hero is not that he has power, but that he has the wisdom and the maturity to use the power wisely. From an acting point of view, that's how I approached the part. - Christopher Reeve
