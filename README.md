``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Never doubt that a small group of thoughtful, committed people can change the world. Indeed. It is the only thing that ever has. - Margaret Mead
