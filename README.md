``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Life a culmination of the past, an awareness of the present, an indication of the future beyond knowledge, the quality that gives a touch of divinity to matter. - Charles Lindbergh
