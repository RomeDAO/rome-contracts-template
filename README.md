# Boilerplate for RomeDAO solidity smart contract development

fork of [template-ethereum-contracts](https://github.com/wighawag/template-ethereum-contracts) made to run with forge instead of dapptools.

## INSTALL

```bash
yarn
```

## RUN

```bash
yarn dev
```

## TEST

```bash
yarn test
```

The tests are run with forge which requires forge to be installed.

Install forge by following the instructions [here](https://github.com/gakonst/foundry)

## SCRIPTS

Here is the list of npm scripts you can execute:
<br/><br/>

### `yarn dev`

These will run a local hardhat network on `localhost:8545` and deploy your contracts on it. Plus it will watch for any changes and redeploy them.
<br/><br/>

### `yarn test`

This will execute forge tests located in `src/tests`
<br/><br/>

### `yarn execute <network> <file.ts> [args...]`

This will execute the script `<file.ts>` against the specified network.
This command relies on [./\_scripts.js](./_scripts.js) to allow parameterizing it via command line argument
<br/><br/>

### `yarn prepare`

As a standard lifecycle npm script, it is executed automatically upon install. It generate config file and typechain to get you started with type safe contract interactions
<br/><br/>

### `yarn lint`, `yarn lint:fix`, `yarn format` and `yarn format:fix`

These will lint and format check your code. the `:fix` version will modifiy the files to match the requirement specified in `.eslintrc` and `.prettierrc.`
<br/><br/>

### `yarn void:deploy`

This will deploy your contracts on the in-memory hardhat network and exit, leaving no trace. quick way to ensure deployments work as intended without consequences
<br/><br/>
