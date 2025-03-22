``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Judge nothing, you will be happy. Forgive everything, you will be happier. Love everything, you will be happiest. - Sri Chinmoy
