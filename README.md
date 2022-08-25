koa-ejs
========

prettier will crash the code , so fork repo from https://github.com/koajs/ejs , make them compatable.

# install

```
npm install koa-ejs2
```


## how to use ejs with prettier

1. use `<%&JSON.stringify(obj)%>` instead of `<%&JSON.stringify(obj)%>`

2. change `openDelimiter` and `closeDelimiter`

example: 
```
render(app, {
    root: path.join(__dirname, "views"),
    layout: "layout",
    viewExt: "html",
    map: { html: "ejs" },
    cache: false,
    debug: false,
    openDelimiter: "[",
    closeDelimiter: "]",
});
```

>now you can enjoy prettier in ejs.
