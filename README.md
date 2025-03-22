``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Look back over the past, with its changing empires that rose and fell, and you can foresee the future, too. - Marcus Aurelius
