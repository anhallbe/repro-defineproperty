# ReproDefineproperty

## Steps to reproduce:

1. `npm ci`
2. `ng serve --configuration production`
3. Go to `http://localhost:4200` in the browser
4. Open the Developer Tools console, see the error

## Steps taken to produce this code:

1. `ng new repro-defineproperty`
2. `npm i ids-enterprise-wc@1.0.0-beta.9`
3. Added `import "ids-enterprise-wc"` to `main.ts`
4. Added `skipLibCheck` to `tsconfig.json` because for some reason the `"dom"` lib isn't found when compiling with Angular.
