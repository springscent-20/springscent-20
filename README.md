``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## With the realization of one's own potential and self-confidence in one's ability, one can build a better world. - Dalai Lama
