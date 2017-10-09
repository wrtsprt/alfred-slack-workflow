# Setting up credentials

You can generate a Slack legacy token here: https://api.slack.com/custom-integrations/legacy-tokens

Your credentials should be safely stored inside the OS X keychain.
To do this open Keychain Access (open spotlight, type Keychain). Select the login keychain.
Click the plus on the bottom to add an account.

Keychain item name: slack-af-legacy-token Account Name: doesntmatter Password: <yourlegacytoken>

Click Add.

Now open your terminal an call `security find-generic-password -l slack-af-legacy-token -w` once.
This will attempt to retrieve your password from Keychain and will popup the permissions dialog.
Pleaes select Always allow, for the workflow to be able to retrieve the credentails later on.
