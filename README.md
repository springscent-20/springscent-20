``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## The most important thing is transforming our minds, for a new way of thinking, a new outlook: we should strive to develop a new inner world. - Dalai Lama
