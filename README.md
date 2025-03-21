``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Every person, all the events of your life are there because you have drawn them there. What you choose to do with them is up to you. - Richard Bach
