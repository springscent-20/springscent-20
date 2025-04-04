``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## A lot of times people look at the negative side of what they feel they can't do. I always look on the positive side of what I can do. - Chuck Norris
