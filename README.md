``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## I have been impressed with the urgency of doing. Knowing is not enough; we must apply. Being willing is not enough; we must do. - Leonardo da Vinci
