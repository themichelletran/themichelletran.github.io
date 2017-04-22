# Resume Site

## Building/Deploying
Because of Github's constraints on using the `master` branch for personal GH pages, this branch hosts all the source files and the Blendid instance.

Blendid's `ghPages` task generates the build files to the `gh-pages` branch, so this requires a couple steps to deploy.

```bash
git co source
yarn blendid -- ghPages
git co master
git reset --hard gh-pages
git push
```
