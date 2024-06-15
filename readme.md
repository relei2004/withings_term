This is a small, simple script to read your weight and steps from your Withings account. The script saves the weight and steps in a file, so you don't need to make a roundtrip to your Withings account every time. This way, you can schedule this script in crontab. I use this script to show my weight and steps in dwmblocks.

# How to Get Your Client ID, Secret, and Callback URL from Withings

1. Go to: [Withings Developer](https://developer.withings.com/)
2. Click "Sign In / Go to Developer Dashboard".
3. Click "Public Cloud".
4. Log in with your credentials.
5. Click "Create an Application".
6. Select "I don’t know yet" and click "Next".
7. Enter an Application name, Description, and a Callback URL (you don't have to use a real URL).
8. You will now have all you need: a Client ID, Secret, and the Callback URL. Copy all three into your script.

# Usage
The first time you start the script, you have to log in with your browser to your Withings account. Follow the instructions provided by the script. After that, the script automatically renews the login token and saves all information for login in the `withings_tokens.json`.

You can start the script with these options:
- `-w` to get the weight
- `-s` to get the steps
- `-l` to get both in one line
- `-i` adds the corresponding icon to the values; you can combine it with `-w`, `-s`, and `-l`

