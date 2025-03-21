``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## You can tell whether a man is clever by his answers. You can tell whether a man is wise by his questions. - Naguib Mahfouz
