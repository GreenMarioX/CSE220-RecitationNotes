# Setting Up SSH on GitHub

This tutorial will guide you through the process of setting up SSH on GitHub for both Mac and Windows operating systems.

SSH is not mandatory to set up if you are using codespaces or if you are cloning via https.

## GitHub Documentation
The following tutorial was written based on the three links below. Please refer to them for assistance with setting up SSH.

- [Generating a new SSH key and adding it to the SSH agent](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

- [Adding a new SSH key to your GitHub account (Windows)](https://docs.github.com/en/enterprise-cloud@latest/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account?platform=windows)

- [Adding a new SSH key to your GitHub account (Mac)](https://docs.github.com/en/enterprise-cloud@latest/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account?platform=mac)

## Prerequisites
Before you begin, make sure you have the following:

- A GitHub account
- Git installed on your machine

## Mac Setup
Follow these steps to set up SSH on GitHub for Mac:

1. Open Terminal on your Mac.
2. Generate a new SSH key by running the following command:
    ```
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
    ```
    Replace "your_email@example.com" with your GitHub email address.
3. Press Enter to accept the default file location and enter a passphrase if desired.
4. Start the SSH agent by running the following command:
    ```
    eval "$(ssh-agent -s)"
    ```
5. Add your SSH private key to the SSH agent by running the following command:
    ```
    ssh-add -K ~/.ssh/id_rsa
    ```
6. Copy your SSH public key to the clipboard by running the following command:
    ```
    pbcopy < ~/.ssh/id_rsa.pub
    ```
7. Go to your GitHub account settings and navigate to [SSH and GPG keys](https://github.com/settings/keys).
8. Click on "New SSH key" and paste your public key into the "Key" field.
9. Give your SSH key a descriptive title and click "Add SSH key".

## Windows Setup
Follow these steps to set up SSH on GitHub for Windows:

1. Open Git Bash on your Windows machine.
2. Generate a new SSH key by running the following command:
    ```
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
    ```
    Replace "your_email@example.com" with your GitHub email address.
3. Press Enter to accept the default file location and enter a passphrase if desired.
4. Start the SSH agent by running the following command:
    ```
    eval "$(ssh-agent -s)"
    ```
5. Add your SSH private key to the SSH agent by running the following command:
    ```
    ssh-add ~/.ssh/id_rsa
    ```
6. Copy your SSH public key to the clipboard by running the following command:
    ```
    cat ~/.ssh/id_rsa.pub | clip
    ```
7. Go to your GitHub account settings and navigate to [SSH and GPG keys](https://github.com/settings/keys).
8. Click on "New SSH key" and paste your public key into the "Key" field.
9. Give your SSH key a descriptive title and click "Add SSH key".

That's it! You have successfully set up SSH on GitHub for both Mac and Windows.

## Troubleshooting
If you are having trouble with setting up SSH, either come to TA office hours, follow a YouTube tutorial, or utilize the official GitHub documentation.

