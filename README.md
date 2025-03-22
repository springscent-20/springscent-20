``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## The teacher who is indeed wise does not bid you to enter the house of his wisdom but rather leads you to the threshold of your mind. - Kahlil Gibran
