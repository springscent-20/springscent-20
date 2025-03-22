``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## If you look into your own heart, and you find nothing wrong there, what is there to worry about? What is there to fear? - Confucius
