``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## By letting it go it all gets done. The world is won by those who let it go. But when you try and try. The world is beyond the winning. - Laozi
