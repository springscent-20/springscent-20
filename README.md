``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Let us resolve to be masters, not the victims, of our history, controlling our own destiny without giving way to blind suspicions and emotions. - John F. Kennedy
