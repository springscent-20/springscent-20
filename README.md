``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## You learn to speak by speaking, to study by studying, to run by running, to work by working; in just the same way, you learn to love by loving. - Anatole France
