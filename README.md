``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Knowledge is going to make you stronger. Knowledge is going to let you control your life. Knowledge is going to give you the wisdom to teach their children. Knowledge is the thing that makes you smile in the face of disaster. - Avery Brooks
