``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## I do not believe in a fate that falls on men however they act; but I do believe in a fate that falls on man unless they act. - G. K. Chesterton
