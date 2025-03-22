``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Most of our pocket wisdom is conceived for the use of mediocre people, to discourage them from ambitious attempts, and generally console them in their mediocrity. - Robert Louis Stevenson
