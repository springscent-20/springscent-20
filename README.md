``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## A leader is best when people barely know he exists, when his work is done, his aim fulfilled, they will say: we did it ourselves. - Laozi
