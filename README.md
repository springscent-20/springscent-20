``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## If you're trying to create a company, it's like baking a cake. You have to have all the ingredients in the right proportion. - Elon Musk
