``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Not every difficult and dangerous thing is suitable for training, but only that which is conducive to success in achieving the object of our effort. - Epictetus
