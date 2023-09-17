# Connecting to GitHub SSH with Linux

## Making the public/private keys
* To make the public and private keys do:
  * `$ . ./makeSSHKey.sh example@mail.com`
* The assuming that default settings are used, the SSH private and public keys reside in the `~/.ssh directory.`

## Adding the public SSH key to GitHub
* To use the SSH keys, first add the public key (the one that ends in .pub) to the GitHub account.
  * view the public key and copy it `$ cat ~/.ssh/PUBLICKEY.pub`
  * Go to https://github.com/settings/keys and click **New SSH key**
  * Give the key title any name you wish, and paste the key into it.

 ## Starting the verification agent process
* Use the second bash script **connectSSH.sh** to start the verification agent and add the private key in the following way:
  * Navigate to the project directory and enter the following command in the terminal: `$ . ./connectSSH.sh`
