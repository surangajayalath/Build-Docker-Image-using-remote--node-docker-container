# Build Docker image using remote node running container
## Step 1 -> Make private & public key and connect

* Create Keys
* Note: add key name while creating key
```
ssh-keygen -m PEM
```
* share public key to remote machine
* check .ssh folder in remote machine(ls -la)
* below ine send public key to remote machine
```
ssh-copy-id -i sura-key suranga@192.168.143.12
```
* try to connect to remote machine using private key
```
ssh -i sura-key 192.168.143.12
```

## Step 2 -> Set up credential in Jenkins and test connection
## Step 3 -> Build Pipeline with docker
