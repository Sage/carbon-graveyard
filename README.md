# Carbon Graveyard

:skull: Where code comes to die.

All components and modules in this repository are no longer actively maintained, but are available for use if your application heavily relies on them. Ideally you should look to remove any dependency on this code.

Any code contributed to this repository should feature an associated README file with instructions on why it was deprecated and what alternatives you should look to use.

## Making a Release

* Update the version. You can either do this manually in the `package.json` file and run `npm install` to update the `package-lock.json` file, or you can run `npm version x.x.x --no-git-tag-version`.
* Generate the release notes: `./script/generate-release-notes.sh`.
* Create a pull request with your changes into the `release` branch.
* Once merged create a tag in GitHub from `release` for your new version number.
* Check the `release` branch out locally and ensure the code is all up to date, publish the tag to npm with `npm publish`.
* Merge `release` back into `master` to finish the release.