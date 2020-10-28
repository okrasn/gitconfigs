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
