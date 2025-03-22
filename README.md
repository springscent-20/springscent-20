``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Parents can only give good advice or put them on the right paths, but the final forming of a person's character lies in their own hands. - Anne Frank
