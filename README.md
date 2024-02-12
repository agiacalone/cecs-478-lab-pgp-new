# CECS 478 Lab: PGP Encryption (2024 Edition)

## Assignment Description
This assignment is designed to demonstrate how PGP encryption works by using open-source and *auditable* tools to encrypt email messages. It will work equally well on just about any plain-text message.

Install [GnuPG](https://gnupg.org/) in your virtual machine image (use apt--your package manager on Linux Mint, not the website download) and create a public/private key pair. The command `sudo apt install gnupg` should install the requisite programs on your virtual machine. Github has some [good documentation on how to do this here](https://docs.github.com/en/authentication/managing-commit-signature-verification/generating-a-new-gpg-key).

You will generate a public and private key paring using GnuPG. For our assignment, you will need to do the following:

1. Install GnuPG as described above
2. Clone your assignment repository (this one!) to your virtual machine
3. Generate your public and private key pair
4. Decrypt the message included in `secret_message.asc` using my public key `public_key.asc` and your private key `private_key_student.asc` (**Note!**: All file names must be *exact* in this assignment!)
5. Read the message
6. Encrypt the *exact same message* back to my by using your private key `private_key_student.asc` and my public key `public_key.asc` as the file `secret_message_response.asc`
7. Copy your public key `public_key_student.asc` to the repository
8. Copy the newly created `secret_message_response.asc` to the repository
9. **DO NOT INCLUDE ANYTHING ELSE IN THE REPOSITORY**, including your secret key and the decrypted message. Including either of these will cause you to lose 50% of the points for this assignment!
10. Commit and push your repository to Github
11. Enjoy your favorite beverage, as you are done!

## Deliverables
Your final commit and push with the files `public_key_student.asc` and `secret_message_response.asc` in the root directory (along with the files already included with the repository) is your submission. Don't place your files in any subfolders or subdirectories.
