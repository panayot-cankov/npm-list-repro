# npm-list-repro
Npm list in workspace find modules installed at root level

Clone the repo.
In the root run:
```
npm i
cd workspace-a
npm list --production
```
Npm list will throw errors.

Then still in the `worspace-a`:
```
npm i
npm list --production
```
Npm list will not throw errors.

For workspaces, `vsce` seems to need a version of `npm list --production` that will work without installing locally.