# How to start work with Github

Pre condition: Setup Git

## Git configuration

1. Generate SSH keys
    - Register on Github.com
    - Open Git Bash
    - Paste the command below, replace with amplify email address

      `ssh-keygen -t rsa -b 4096 -C "nsurname@mail.com"`

    - When you're prompted to `Enter a file in which to save the key,` press `Enter`. This accepts the default file location.
    - At the prompt, type a secure passphrase
2.  Add SSH key to the ssh-agent
    - Put in the termial

      `eval \$(ssh-agent -s)`

    - Add your SSH private key to the ssh-agent

      `ssh-add ~/.ssh/id_rsa`
3.  Add a new SSH key to GitHub account
    - Copy the SSH key to your clipboard
    
      `clip < ~/.ssh/id_rsa.pub`

    - In the upper-right corner of any page in GitHub, click your profile photo, then click Settings
    - In the user settings sidebar, click SSH and GPG keys
    - Click New SSH key or Add SSH key
    - In the "Title" field, add a descriptive label for the new key. For example, if you're using a personal Mac, you might call this key "Personal MacBook Air"
    - Paste your key into the "Key" field
    - Click Add SSH key
    - If prompted, confirm your GitHub password

4.  Authorizing an SSH key for use with SAML single sign-on(with your project)
    - In the upper-right corner of any page, click your profile photo, then click Settings
    - In the user settings sidebar, click SSH and GPG keys
    - Next to the SSH key you'd like to authorize, click Enable SSO
    - Click Authorize
