``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## When a friend is in trouble, don't annoy him by asking if there is anything you can do. Think up something appropriate and do it. - A. Powell Davies
