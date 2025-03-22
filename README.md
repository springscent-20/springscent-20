``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## You are a product of your environment. So choose the environment that will best develop you toward your objective. Analyze your life in terms of its environment. Are the things around you helping you toward success - or are they holding you back? - W. Clement Stone
