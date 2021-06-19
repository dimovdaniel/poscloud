# Custom CSS

The preferd way to change the CSS is to inspect the elemtn, find the class and overwrite its css styling via the Admin-&gt;Settings-&gt;CSS & JS tab. There you can define your own CSS styling overwrite.

For example, let's change the frontpage initial blue theme to red. This is the CSS you need.

```text
.bg-primary  {
    background-color: #ff0000 !important;
}

.headroom--not-top.navbar-theme-primary {
    background-color: #ff0000 !important;
}

.btn-primary {
    background-color: #ff0000  !important;
}
```

And you can do this for every ID or class inside the HTML.

