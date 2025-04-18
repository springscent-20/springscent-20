``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## One's philosophy is not best expressed in words; it is expressed in the choices one makes... and the choices we make are ultimately our responsibility. - Eleanor Roosevelt
