# npm-release

A little script to help release `npm` modules. It:

- Bumps the version in `package.json`
- Commits 'chore(release): Release vX.X.X-X'
- Tags
- Pushes the commit & tag (`git push && git push --tags`)
- Releases to npm (with `npm publish`)

Does all of the above automatically based on commit messages since the last release. Commits should be using the AngularJS Commit Guidelines, as this package will use the type of the commits to decide the next version.

[Semantic-release][s-r] is a great tool, but if you aren't on Github (and possibly Gitlab) you might be out of luck.

## Usage

You must use `npm-release` in a folder with a `package.json` and a remote to push to.

## Install

`npm install -g npm-release`

## License

MIT

[s-r]: https://github.com/semantic-release/semantic-release
