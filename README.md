# Create Contract App

Provides a command for creating smart-contract projects.

## Features

- [ ] No need to write build configuration.
- [ ] Generate `typescript declaration` for your smart contracts.
- [ ] Doctor your project structure and dependencies.
- [ ] `console.log` in `*.sol`.

## Usage

**First**, generate a project

```sh
npx create-contract-app my-contract-app
```

It will create a directory called `my-contract-app` inside the current folder.

```
my-contract-app
├── contract.config.js
├── contracts
│   ├── MyToken.sol
│   └── MyNFT.sol
└── test
    ├── MyToken.js
    └── MyNFT.js
```

**Second**, go into your project newly created folder:

```sh
cd my-contract-app
```

**Third**, run some built-in commands:

### `npm run doctor` run a checklist

- [ ] Check for environment requirements.
- [ ] Check your project structure.

### `npm run build`

- [ ] Builds smart contracts in `./contracts/**/*.sol`
- [ ] Generate typescript for the ouput ABIs

### `npm test`

- [ ] Run tests in `./test/**/*.js`

### `npm run deploy:<network>`

- [ ] Deploy your contract to a specified network
- [ ] Show a warning/confirmation for dangerous actions
