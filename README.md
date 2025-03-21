``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## It is important to our friends to believe that we are unreservedly frank with them, and important to friendship that we are not. - Mignon McLaughlin
