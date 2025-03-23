``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Knowledge is knowing that a tomato is a fruit. Wisdom is knowing not to put it in a fruit salad. - Brian O'Driscoll
