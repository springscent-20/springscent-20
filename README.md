``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## People usually compare the computer to the head of the human being. I would say that hardware is the bone of the head, the skull. The semiconductor is the brain within the head. The software is the wisdom. And data is the knowledge. - Masayoshi Son
