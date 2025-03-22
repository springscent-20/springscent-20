``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Wherever a man may happen to turn, whatever a man may undertake, he will always end up by returning to the path which nature has marked out for him. - Johann Wolfgang von Goethe
