``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## You may say I'm a dreamer, but I'm not the only one, I hope someday you will join us, and the world will live as one. - John Lennon
