``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Without passion man is a mere latent force and possibility, like the flint which awaits the shock of the iron before it can give forth its spark. - Henri-Frédéric Amiel
