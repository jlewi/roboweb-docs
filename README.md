# website
Roboweb website


## Build static pages

```
cd roboweb
hugo -D
```

Static page will be in public directory

The `-D` option causes drafts to be published.


To start the server

```
cd roboweb
hugo server -D
```


## Publishing

* GitHub actions are used to automatically generate the static site and check it in on
  the gh-pages branch

  * See Hugps [Host on GitHub Docs](https://gohugo.io/hosting-and-deployment/hosting-on-github/)

* The website is published using GitHub pages

## DNS

* Followed [GitHub Pages Custom Domain](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site) instructions to 

  * Setup an APEX domain for roboweb.app
  * Use a CNAME record for www.roboweb.app

# References

[Hugo Quick Start](https://gohugo.io/getting-started/quick-start/)