``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Iron rusts from disuse; water loses its purity from stagnation... even so does inaction sap the vigor of the mind. - Leonardo da Vinci
