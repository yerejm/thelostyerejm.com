# How to set up the site

1. Actions on Github ([Github instructions](https://help.github.com/articles/setting-up-a-custom-domain-with-github-pages/))
  1. Create a repository `<account>.github.io`
  2. Add `index.html` file
  3. Add `CNAME` file containing the domain name (domain.com)
2. Actions on the DNS provider ([Github instructions](https://help.github.com/articles/tips-for-configuring-an-a-record-with-your-dns-provider/))
  1. Create A records
    - `@: 185.199.108.153`
    - `@: 185.199.109.153`
    - `@: 185.199.110.153`
    - `@: 185.199.111.153`
  2. Create CNAME record
    - `www: <account>.github.io.`
3. Wait on:
  - DNS propagation - check with `dig domain.com +nostats +nocomments +nocmd`
  - Github to recognise the site repository
