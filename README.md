``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Perseverance is a great element of success. If you only knock long enough and loud enough at the gate, you are sure to wake up somebody. - Henry Wadsworth Longfellow
