``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## The really unhappy person is the one who leaves undone what they can do, and starts doing what they don't understand; no wonder they come to grief. - Johann Wolfgang von Goethe
