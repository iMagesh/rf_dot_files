# Git Pre Commit Hooks
​
The pre-commit hook is run first, before you even type in a commit message. It’s used to inspect the snapshot that’s about to be committed, to see if you’ve forgotten something, to make sure tests run, or to examine whatever you need to inspect in the code. Exiting non-zero from this hook aborts the commit, although you can bypass it with git commit --no-verify. You can do things like check for code style (run lint or something equivalent), check for trailing whitespace (the default hook does exactly this), or check for appropriate documentation on new methods
​
​
## husky
​
https://www.npmjs.com/package/
​
````
npm install husky --save-dev
npm pkg set scripts.prepare="husky install"
npm run prepare
npx husky add .husky/pre-commit "npm test"
git add .husky/pre-commit
````

https://typicode.github.io/husky/#/

## pre-commit

````
pip install pre-commit
       or
brew install pre-commit (if on MacOS)       
````

Refer - https://pre-commit.com/
