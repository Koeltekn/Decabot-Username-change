# Change your username on deca.art

- Login into your profile
- Open chrome dev tools
  - control + shift + i on windows
  - command + option + i on macOs
  
- Click on the console tab
- Paste the following

```fetch("https://deca.art/api/web/user", {
  "headers": {
    "accept": "*/*",
    "accept-language": "it-IT,it;q=0.9,en-US;q=0.8,en;q=0.7,ja;q=0.6,de;q=0.5",
    "content-type": "text/plain;charset=UTF-8",
    "sec-ch-ua": "\" Not A;Brand\";v=\"99\", \"Chromium\";v=\"100\", \"Google Chrome\";v=\"100\"",
    "sec-ch-ua-mobile": "?0",
    "sec-ch-ua-platform": "\"macOS\"",
    "sec-fetch-dest": "empty",
    "sec-fetch-mode": "cors",
    "sec-fetch-site": "same-origin"
  },
  "referrer": "https://deca.art/test",
  "referrerPolicy": "strict-origin-when-cross-origin",
  "body": "{\"json\":{\"pfp\":null,\"decagon\":null,\"banner\":null,\"username\":\"AAAAAAAAAAAAAA\",\"bio\":null,\"badges\":null},\"meta\":{\"values\":{\"pfp\":[\"undefined\"],\"decagon\":[\"undefined\"],\"banner\":[\"undefined\"],\"bio\":[\"undefined\"],\"badges\":[\"undefined\"]}}}",
  "method": "POST",
  "mode": "cors",
  "credentials": "include"
});
```

- Replace AAAAAAAAAAAAAA with your new username
- Press enter
- If you see no red text, your username is now changed
