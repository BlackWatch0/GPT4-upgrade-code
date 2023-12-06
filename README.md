# GPT4-upgrade-code
This code can skip the waitline for gptplus

```javascript
fetch("/api/auth/session").then(r => r.json()).then(({ accessToken }) => {
    fetch("/backend-api/payments/checkout", {
        method: "POST",
        headers: {
            "authorization": `Bearer ${accessToken}`,
        },
    }).then(r => r.json()).then(d => window.open(d.url));
});
```

use this code in console(press F12 in the chatgpt page with your account login in)
**available in 6/12/2023**
STAR THIS REPOSITORY IF YOU SUCCESSED
