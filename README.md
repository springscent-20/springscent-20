``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## An optimist is a person who sees a green light everywhere, while the pessimist sees only the red spotlight... The truly wise person is color-blind. - Albert Schweitzer
