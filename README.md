### SafeDrive: Data-Driven Simulations and Multi-Agent Interactions for Autonomous Vehicle Safety
Workshop website template

## Build
1. Install [Hugo](https://gohugo.io/)
2. Clone the repo
```
git clone https://github.com/safeav/safeav.github.io.git
cd safeav.github.io
```
3. Run `hugo` in the `pwd`. This will build the website
4. To watch on localhost, run `hugo server --watch`. This is will give a localhost link.

## Adding Data
1. `index.html` in `layout/` is to be edited/changed.
2. `index.html` in `static/categories` is to be edited/changed. Replace the ml4ad with our website.
3. Adding the images content in `static/img`.
4. `index.html` in `static/tags` is to be edited/changed. Replace the ml4ad with our website.

## Deploying
`Note: Verify locally first and then push to github`

1. Run `hugo` in `pwd`, after editing the files. This will generate the `public` folder, which is then used for the deployment.
2. Steps to push local data to the remote
```
git init
git checkout main
git add .
git commit -m "message what is being updated"
git push origin main
```
3. We are using `gh-pages` for the deployment.
```
cd public/
git init
git checkout gh-pages
git add .
git commit -m "message what is being updated"
git push origin gh-pages
```
4. The website will be live with the changes at [https://safeav.github.io/]