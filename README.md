``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## If one is estranged from oneself, then one is estranged from others too. If one is out of touch with oneself, then one cannot touch others. - Anne Lindbergh
