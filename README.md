``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## The key to wisdom is this - constant and frequent questioning, for by doubting we are led to question and by questioning we arrive at the truth. - Peter Abelard
