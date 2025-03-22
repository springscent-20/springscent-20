``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## I'm astounded by people who want to 'know' the universe when it's hard enough to find your way around Chinatown. - Woody Allen
