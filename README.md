# gh-pages-secret-poc

Steps to create a secret gh-pages

1) Create a new private repo with a super secret token (maybe try [randomkeygen](http://randomkeygen.com/))

2) Add new remote to existing repo:

```sh
git remote add secret git@github.com:Hypercubed/290182e185f15ec57c927e7742805594.git
```

3) Publish gh-pages to new repo (use git directly or gulp-gh-pages, etc).  For example:

```sh
git checkout -b gh-pages
git push secret gh-pages
```

4) Send your secret gh-pages to friends: [http://hypercubed.github.io/290182e185f15ec57c927e7742805594/](http://hypercubed.github.io/290182e185f15ec57c927e7742805594/)

5) Keep up-to-date by pushing `gh-pages` to secret, never to master.  Example:

```sh
git push secret master:gh-pages
```
