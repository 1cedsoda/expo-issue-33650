# Expo Issue 33650 Reproduction

```bash
# Create expo app with SDK 52.0.18 at the time
npx create-expo-app@latest repro
cd repro
npm i
npx expo install --fix
npm run start
```

Error message:

```bash
Error: /Users/redacted/node_modules/expo-updates/build-cli/cli.js:46
commands[command]().then((exec) => exec(commandArgs));
                 ^

TypeError: commands[command] is not a function
    at Object.<anonymous> (/Users/redacted/node_modules/expo-updates/build-cli/cli.js:46:18)
    at Module._compile (node:internal/modules/cjs/loader:1256:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1310:10)
    at Module.load (node:internal/modules/cjs/loader:1119:32)
    at Module._load (node:internal/modules/cjs/loader:960:12)
    at Module.require (node:internal/modules/cjs/loader:1143:19)
    at require (node:internal/modules/cjs/helpers:119:18)
    at Object.<anonymous> (/Users/redacted/node_modules/expo-updates/bin/cli.js:3:1)
    at Module._compile (node:internal/modules/cjs/loader:1256:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1310:10)

Node.js v18.18.2
```
