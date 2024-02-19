# Apache2 Example

This example is deploys a site using [Apache2 HTTP Server](https://httpd.apache.org/)

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template/o3MbZe)


## ✨ Features

- Apache2
- Static Site

## 💁‍♀️ How to use

- Open the `site/index.html` in the browser

## 📝 Notes

By default the `site/` directory gets deployed as a static site. This can be modified by changing the `Dockerfile`.

The site is deployed using the default Apache 2 HTTP configuration. This can be overridden with a custom conf file by adding

```
FROM httpd:2.4
COPY ./my-httpd.conf /usr/local/apache2/conf/httpd.conf
```

to the end of the Dockerfile. For more information, [read the docs](https://hub.docker.com/_/httpd).
