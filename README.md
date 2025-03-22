``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Treat people as if they were what they ought to be, and you help them to become what they are capable of being. - Johann Wolfgang von Goethe
