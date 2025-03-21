``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## If a man does not make new acquaintances as he advances through life, he will soon find himself left alone. A man, sir, should keep his friendship in a constant repair. - Samuel Johnson
