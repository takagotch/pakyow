### pakyow
---
https://www.pakyow.org/

https://github.com/pakyow/pakyow


```
gem install pakyow
pakyow new webapp
cd webapp
bundle exec pakyow server
curl http://localhost:3000
```

```
<div@post>
  <p@body> goes here</p>
</div>

<div@post>
  <h1@title></h1>
</div>

<div@post>
  <h1@title></h1>
  <p@body></p>
</div>

<div@post>
  <h1@title></h1>
</div>
```

```ruby
view.find(:post)
view.find(:post, :body, ...)
view.find(:post).find(:body).find(...)

view.with do |view|
end

view.container(:foo)
view.partial(:foo)
view.component(:foo)
view.form(:post)

view.bind(post: { title: "..." })
view.find(:post).bind(title: "...")

view.find(:post).transform(title: "foo")
```


