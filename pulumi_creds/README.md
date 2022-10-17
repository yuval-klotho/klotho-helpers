# Pulumi credentials dir

Put your Pulumi personal access tokens here, and `pulumi-login` will recognize them.

**Do not check files into this directory.** This readme file should be the only file in this dir that git knows about.

Each file should contain only one line, which is the Pulumi personal access token.

## To add a token

1. Navigate to https://app.pulumi.com
2. Click on "access tokens" in the left pane
3. Click "create token" in the top-right corner
4. Give your token a name (doesn't matter what).
5. Copy the token (which should start `pul-*`) into a file in this directory.
  - The file name (including any suffixes) will be the name that `pulumi-login` uses.
  - **Important**: Do not paste your token into the termainal; e.g., do not do `echo pul-123f > myfile`. If you do, your token will be in your bash history. Instead, open the file in your favorite text editor, and paste the contents in there. On Mac, you can also write it directly from your clipboard: `pbpaste > myfile`
