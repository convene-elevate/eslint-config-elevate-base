# eslint-config-elevate-base

Elevate's base JS ESLint config.

## How to configure

1) npm install https://github.com/convene-elevate/eslint-config-elevate-base.git#actual_version --save-dev
2) npm install eslint@4.16.0 --save-dev
3) In you project root you need to add .eslintrc file with a default configuration.
```
{
    "extends": "eslint-config-elevate-base"
}
```
4) You can add .eslintignore file if you need to configure scopes, those need to be ignored by your linter. For example:
```
**/node_modules/*
```

Read more about the eslint configuration [here](https://eslint.org/docs/user-guide/configuring).

## How to use

1) eslint --ext .js ./app_directory

Read more about the CLI [here](https://eslint.org/docs/user-guide/command-line-interface)

## How to automate linting

1) npm install husky --save-dev
2) Add the next lines in a scripts section in your package.json
```
"lint": "eslint --ext .js ./app_directory",
"precommit": "npm run lint"
```
