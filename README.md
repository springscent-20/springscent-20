``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## There is only one boss. The customer. And he can fire everybody in the company from the chairman on down, simply by spending his money somewhere else. - Sam Walton
