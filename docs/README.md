# ipyauth Docs

This folder contains the documentation, on line at: https://oscar6echo.gitlab.io/ipyauth/

## Develop

Run from terminal:

```bash
$ yarn docs:dev
```


## Deploy

You can manually deploy as follows:

```bash
# build
cd docs
yarn docs:build

# navigate into the build output directory
cd ../public

# you need to remove public/ from .gitignore for manual run
git add .
git commit -m 'deploy'

# you are deploying to https://oscar6echo.gitlab.io/ipyauth
git push -f git@gitlab.com:oscar6echo/ipyauth.git master:pages
# or equivalently
git subtree push --prefix public/ origin pages

# back repo top level
cd ..
```
