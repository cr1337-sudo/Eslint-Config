# Eslint
npm install eslint --save-dev <br>
npm init @eslint/config

# Eslint para React (JS)

## Prettier
npm install --save-dev eslint-config-prettier <br>
npm install --save-dev eslint-plugin-prettier <br>
npm install --save-dev --save-exact prettier

## Autosort imports (ES6 Modules)
npm i eslint-plugin-simple-import-sort -D

# Actualizar código al guardar
Settings.JSON: <br>
"editor.codeActionsOnSave": {"source.fixAll.eslint": true}

# VSC Dependencias
Eslint <br>
CodeLens

# Eslint para backend (TS)

npm i eslint eslint-config-standard-with-typescript -D

## .eslintrc.sjon

```
{
    "extends": "standard-with-typescript",
    "parserOptions": {
        "project": "./tsconfig.json"
    },
    "rules": {
        "@typescript-eslint/quotes": [
            "error",
            "double",
            {
                "allowTemplateLiterals": true
            }
        ],
        "semi": "off",
        "@typescript-eslint/semi": [
            "error",
            "always"
        ],
        // Desactiva error en promesas que no tienen try/catch o then/catch
        "@typescript-eslint/no-floating-promises": "off"
    },
    "ignorePatterns": [
        "dist",
        "src/**/*.js"
    ]
}
```
