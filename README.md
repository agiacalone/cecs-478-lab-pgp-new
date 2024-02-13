# CECS 478 Lab: PGP Encryption (2024 Edition)

## Assignment Description
This assignment is designed to demonstrate how PGP encryption works by using open-source and *auditable* tools to encrypt email messages. It will work equally well on just about any plain-text message.

Install [GnuPG](https://gnupg.org/) in your virtual machine image (use apt--your package manager on Linux Mint, not the website download) and create a public/private key pair. The command `sudo apt install gnupg` should install the requisite programs on your virtual machine. Github has some [good documentation on how to do this here](https://docs.github.com/en/authentication/managing-commit-signature-verification/generating-a-new-gpg-key).

You will generate a public and private key paring using GnuPG. For our assignment, you will need to do the following:

1. Install GnuPG as described above
2. Clone your assignment repository (this one!) to your virtual machine
3. Generate your public and private key pair
4. Place your public key in the project repository folder as `public_key.asc`
5. Commit and push your repository. Wait at least one working day (not weekend day)
6. Pull your repository. There will be at least two new files there named `message_to_student.asc` and `verification.asc` 
7. Decrypt the message included in `message_to_student.asc` using my public key `prof_pkey.asc` and your private key (**Note!**: All file names must be *exact* in this assignment!)
8. Read the message
9. Encrypt the *exact same message* back to my by using your private key and my public key `prof_pkey.asc` as the file `secret_message_response.asc`
10. Place the `secret_message_response.asc` file in the git repository (don't use any sub-directories)
11. **DO NOT INCLUDE ANYTHING ELSE IN THE REPOSITORY**, including your secret key and the decrypted message. Including either of these will cause you to lose 50% of the points for this assignment!
12. Commit and push the repository. Wait another working day or two
13. Pull the repository and you should see a new file named `verdicts.json` and possibly others
14. Read `verdicts.json` and fix any errors
15. Commit, push, repeat until all errors are resolved
16. Enjoy your favorite beverage, as you are done!

## Deliverables
Your final commit and push with the files `public_key.asc`, `message_to_student.asc`, and the final `verdicts.json` in the root directory (along with the files already included with the repository) is your submission. Don't place your files in any subfolders or subdirectories.
