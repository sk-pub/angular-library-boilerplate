# Steps to build a basic Angular library boilerplate

## VS Code: https://code.visualstudio.com/

## Volta: https://docs.volta.sh/guide/getting-started

    volta -v

## Node + NPM (LTS)

    volta install node@18

    node -v

## Angular library:

    ng new basic-library --create-application=false
    cd basic-library
    ng generate library basic-library
    ng build

    ng test

## ESLint:

    cd basic-library
    ng add @angular-eslint/schematics

    ng lint

## StyleLint

    npm install --save-dev stylelint stylelint-config-standard-scss
    .stylelintrc.json https://stylelint.io/user-guide/get-started
    package.json "lint:styles": "stylelint \"**/*.scss\""

    npm run lint:styles

## Prettier

    npm install prettier --save-dev
    .prettierrc.json
    .prettierignore

    See https://prettier.io/docs/en/integrating-with-linters.html
    npm install eslint-config-prettier --save-dev

    npx prettier --check .

## Jest

    // See https://www.justjeb.com/post/angular-cli-ng-test-with-jest
    npm uninstall karma karma-chrome-launcher karma-coverage karma-jasmine  karma-jasmine-html-reporter jasmine-core @types/jasmine
    npm i jest @types/jest @angular-builders/jest --save-dev

    npm test
