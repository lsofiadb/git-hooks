# Git Hooks :gun:
NodeJs project to testing git hooks, husky and lint staged. 

## [Husky](https://typicode.github.io/husky/#/)🐺
You can use it to lint your commit messages, run tests, lint code, etc... when you commit or push. Husky supports all Git hooks. It's kinda a trigger. 

## [Lint staged](https://www.npmjs.com/package/lint-staged) :paperclip:
"Linting makes more sense when run before committing your code. By doing so you can ensure no errors go into the repository and enforce code style. But running a lint process on a whole project is slow, and linting results can be irrelevant. Ultimately you only want to lint files that will be committed."

## Installation 

``` shell
npm install -D husky lint-staged
```

``` shell
npm set-script prepare 'husky install'
```

// Create .husky directory in order to configurate git hooks (pre-commit script for example)
``` shell
 npm run prepare 
```

``` shell 
npx husky add .husky/pre-commit "npx lint-staged"
```

``` shell
npx eslint --init
```