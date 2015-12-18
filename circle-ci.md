# Continuous Deployment with Circle CI
We integrated Circle CI on Dec 17, with the help of Lev Lazinskiy. The following are the steps we took to push the Circle builds to cosmos server:

1. __Getting Started__: Go into the `.ssh` folder in the server
2. __Generate a SSH Key__ using: `ssh-keygen` called `circleci_rsa`
3. __Copy the "Public Key" into clipboard__: `pbcopy < circleci_rsa.pub`
4. __Create and `authorized_keys` file__: still in the `.ssh` folder, `nano authorized_keys`
5. __Paste the public key__ into the the `authorized_keys` file - save the changes you've made, press `Ctrl + O`. To exit nano, type `Ctrl + X`
6. __On your GitHub__: create the `circle.yml` with the test and deployment scripts.
