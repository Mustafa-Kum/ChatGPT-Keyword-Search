# ChatGPT Powered

https://chat.openai.com/chat

```python

import requests

# List of websites to search
websites = ['https://infosecwriteups.com/using-chatgpt-to-create-darkweb-monitoring-tool-7b7eeaab351f', 'https://www.another-example.com']

# Keyword to search for
keyword = 'python'

# Search each website for the keyword
for website in websites:
    try:
        # Send a GET request to the website
        response = requests.get(website)
        # Get the response text
        text = response.text
        # Check if the keyword is in the response text
        if keyword in text:
            print(f'Keyword found on {website}')
        else:
            print(f'Keyword not found on {website}')
    except:
        print(f'Error accessing {website}')
       
```
