``` python
import requests

def get_random_quote():
    response = requests.get("https://api.quotable.io/random", verify=False)
    data = response.json()
    return f"{data['content']} - {data['author']}"

print(get_random_quote())
```

    ## Friendships are the family we make - not the one we inherit. I've always been someone to whom friendship, elective affinities, is as important as family. - Salman Rushdie
