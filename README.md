``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Let go of your attachment to being right, and suddenly your mind is more open. You're able to benefit from the unique viewpoints of others, without being crippled by your own judgement. - Ralph Marston
