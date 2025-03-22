``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## The truth is incontrovertible. Malice may attack it, ignorance may deride it, but in the end, there it is. - Winston Churchill
