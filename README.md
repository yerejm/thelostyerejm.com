# How to set up the site

1. Github
  1. Create a repository `<account>.github.io`
  2. Add `index.html` file
  3. Add `CNAME` file containing the domain name (domain.com)
2. DNS provider
  1. Create 2 A records
    - `@: 192.30.252.154`
    - `@: 192.30.252.153`
  2. Create CNAME record
    - `www: <account>.github.io.`
3. Wait on:
  - DNS propagation - check with `dig domain.com +nostats +nocomments +nocmd`
  - Github to recognise the site repository
