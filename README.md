# How to test

## Test using forked [adaplays](https://github.com/vacuumlabs/nufi-adaplays.xyz) testing dapp
- Open the already installed Metamask-Flask extension and set up your account.
- Navigate to [testing dapp](https://nufi-demo-sso-7c6ea9888095.herokuapp.com/).
- Click `Sign in with Google`.
- Confirm action inside a floating NuFi widget that should appear.
- In the popup that appears choose your Google account and confirm.
- Choose a password.
- Fund your wallet (we are using Cardano preprod network).
- Create a game according to the dapp.
- Sign transaction (prompt should be displayed within the floating Widget).
- Wait until the game move expires.
- Click on `Get your funds back`.
- Sign transaction (prompt should be displayed within the floating Widget).

TODO: link to videos

## Troubleshooting

If experiencing unexpected behavior, please try refreshing the page and repeat the process.
Always `Get your funds back` (see above) after making the move, as otherwise, the dapp may not
work correctly with other accounts.

### Known issues
1. When clicking on `Deny` button the Google button is still in `Connecting ...` state. To resolve
just refresh the page.


In case of any other issues please reach out to us at [TODO: email]
