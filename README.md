``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## True happiness arises, in the first place, from the enjoyment of oneself, and in the next, from the friendship and conversation of a few select companions. - Joseph Addison
