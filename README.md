# Connecting to GitHub SSH using Linux

## Making the public/private keys
* To make the public and private keys do:
  * `. ./makeSSHKey.sh example@mail.com`
* The assuming that default settings are used, the SSH private and public keys reside in the `~/.ssh directory.`

## Using the SSH keys
* To use the SSH keys, first add the public key (the one that ends in .pub) to the GitHub account. 
* Use the second bash script **connectSSH.sh** to start the verification agent and adding the private key in the following way:
 * `. ./connectSSH.sh`
