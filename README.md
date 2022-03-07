
<p><a href="https://dashboard.heroku.com/new?template=https://github.com/WestonLehner/xray-dan"> <img src="https://www.herokucdn.com/deploy/button.svg" alt="Deploy to Heroku" /></a></p>

```js
addEventListener(
    "fetch",event => {
        let url=new URL(event.request.url);
        url.hostname="appname.herokuapp.com";
        let request=new Request(url,event.request);
        event. respondWith(
            fetch(request)
        )
    }
)
```
