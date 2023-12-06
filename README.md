# NuFi SSO Widget

We are looking for further funding for this project through [Catalyst grant](https://cardano.ideascale.com/c/idea/114276)

<img width="1503" alt="Screenshot 2023-12-06 at 09 28 19" src="https://github.com/nufi-official/sso-demo/assets/10008234/99c8f4f0-69a1-4021-817a-fa28e462cf2d">

## How to test

### Test using forked [adaplays](https://github.com/vacuumlabs/nufi-adaplays.xyz) testing dApp

#### Connect
- Please try this prototype in a new Chrome profile (with no extensions) or at least disable all wallet extensions first.
- Navigate to the [testing dapp here](https://nufi-demo-sso-7c6ea9888095.herokuapp.com/).
  * Note: this is just a testing dApp and is not part of our solution.
- Click `Sign in with Google`.
- A NuFi wallet widget should appear; click `Allow`.
- Next, a Web3auth popup should appear; choose your Google account and log in.
- Finally, choose a game password (this is required by the dApp and is unrelated to our product).

#### Fund your wallet
- Fund your wallet by claiming test ADA from this [faucet](https://docs.cardano.org/cardano-testnet/tools/faucet/) (we are using Cardano Preprod, so be sure to select `Preprod Testnet`).
- You can find your wallet’s receiving address in the widget (click Receive).
  * You will have to refresh the dApp page and re-login (by clicking `Sign in with Google` button) to re-load your balance.

#### Tasks
- Inspect the content of the NuFi floating wallet widget.
- Create a game by following the instructions on the dApp.
- The NuFi floating widget should show a `Sign transaction` prompt.
- Sign the transaction.
- Wait until the game move expires.
- Click on Get your funds back.
- The NuFi floating widget should show a `Sign transaction` prompt.
- Sign the transaction.

### Troubleshooting

If experiencing unexpected behavior, please try refreshing the page and repeat the process.
Always `Get your funds back` (see above) after making the move, as otherwise, the dapp may not
work correctly with other accounts.

### Known issues
1. When clicking on `Deny` button the Google button is still in `Connecting ...` state. To resolve
just refresh the page.
