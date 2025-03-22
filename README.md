``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## I prefer to be true to myself, even at the hazard of incurring the ridicule of others, rather than to be false, and to incur my own abhorrence. - Frederick Douglass
