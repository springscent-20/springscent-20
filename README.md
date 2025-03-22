``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## To understand the heart and mind of a person, look not at what he has already achieved, but at what he aspires to do. - Kahlil Gibran
