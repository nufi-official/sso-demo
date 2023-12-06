# NuFi SSO Widget

We are looking for further funding for this project through [Catalyst grant](https://cardano.ideascale.com/c/idea/114276)

<img width="1503" alt="Screenshot 2023-12-06 at 09 28 19" src="https://github.com/nufi-official/sso-demo/assets/10008234/99c8f4f0-69a1-4021-817a-fa28e462cf2d">

## How to test

### Test using forked [adaplays](https://github.com/vacuumlabs/nufi-adaplays.xyz) testing dapp
- Please try this prototype in a new Chrome profile or at least disable all wallet extensions in your Chrome.
- Navigate to [testing dapp](https://nufi-demo-sso-7c6ea9888095.herokuapp.com/).
   * Note that this is just a testing dapp and is not part of the proposal itself.
- Click `Sign in with Google`.
- Confirm action inside a floating NuFi widget that should appear.
- In the web3Auth popup that appears choose your Google account and confirm.
- Choose a password (dapp specific, unrelated to our product).
- Fund your wallet via [faucet](https://docs.cardano.org/cardano-testnet/tools/faucet/) (we are using Cardano preprod network).
  * You will have to refresh the dapp page and re-login with `Sign in with Google` button to reload your balance.
- Inspect the content of the NuFi floating widget.
- Create a game according to the dapp.
- The NuFi floating widget should show a sign transaction prompt.
- Sign transaction.
- Wait until the game move expires.
- Click on `Get your funds back`.
- The NuFi floating widget should show a sign transaction prompt.
- Sign transaction.

### Troubleshooting

If experiencing unexpected behavior, please try refreshing the page and repeat the process.
Always `Get your funds back` (see above) after making the move, as otherwise, the dapp may not
work correctly with other accounts.

### Known issues
1. When clicking on `Deny` button the Google button is still in `Connecting ...` state. To resolve
just refresh the page.
