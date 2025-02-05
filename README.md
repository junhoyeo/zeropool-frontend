# Wallet

In actual version (0.22.9) we only support Goerli test network. Wallet awailable [here](https://goerli.testnet.frontend.v2.zeropool.network/).

<!-- # Important! How to run project:

## 1. Clone
- `git clone https://github.com/zeropoolnetwork/zeropool-frontend.git`

## 2. Init
In standalone terminal (use gitbush on Windows) run this commands from the root folder of the project:
- `./scripts/start-local` - start the app dev server

If blockchain node process halted remove it (from powershell if needed):

- netstat -ano | findstr :8545
- taskkill /PID [Process Id] /F  -->

# Developement

First of all, in the project directory create static/assets/ folder and put there respective static files from [this repo](https://github.com/zeropoolnetwork/zeropool-frontend-static.git)

Then in the project directory select the network you want to work with:

##### `mklink .env .env.near` - select NEAR (Windows command prompt as admin)

##### `ln -s .env.near .env` - select NEAR (Linux)

##### `mklink .env .env.goerli` - select Goerli (Windows command prompt as admin)

##### `ln -s .env.goerli .env` - select Goerli (Linux)

After that you can run the following commands:

## `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

## `yarn test:debug`

Launches the test runner in the interactive watch mode.

## `yarn test:debug [part_of_the_file_name]`

Launches the test runner in the interactive watch mode for the specified file(-s).

## `yarn test`

Build the test coverage report.

## `yarn coverage`

Runs local server to show test coverage report.
