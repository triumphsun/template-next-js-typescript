## Next.js
```bash
npx create-next-app@latest --typescript

✔ What is your project named? … template-next-js-typescript
✔ Would you like to use ESLint? … Yes
✔ Would you like to use Tailwind CSS? … No
✔ Would you like to use `src/` directory? … Yes
✔ Would you like to use App Router? (recommended) … Yes
✔ Would you like to customize the default import alias (@/*)? … No
```

## Husky & Lint-staged
```bash
npm install -D husky lint-staged

# run only once after installation
npm pkg set scripts.prepare="husky install"
npm run prepare

# create a pre-commit hook
npx husky add .husky/pre-commit "npm test"
git add .husky/pre-commit

vim .lintstagedrc.json
git add .lintstagerc.json
```

## ESLint
```bash
npm init @eslint/config
# It will automatically install the following modules at the devDependencies: 
#        eslint-plugin-react@latest 
#        @typescript-eslint/eslint-plugin@latest 
#        @typescript-eslint/parser@latest
#

# eslint-config
npm install -D eslint-config-airbnb eslint-config-airbnb-typescript

# eslint-plugin
npm install -D eslint-plugin-simple-import-sort
npm install -D eslint-plugin-unused-imports
npm install -D eslint-plugin-react eslint-plugin-react-hooks

vim .eslintrc.json
git add .eslintrc.json 
```