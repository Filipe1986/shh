# shh
MAC
  check the OpenSSH client version
  ```
  ssh -V 
  ```  
  List keys
  ```
  ls ~/.ssh/*.pub
  ```
  Generate the keys
  ```
  ssh-keygen -t ed25519
  ```
  
  Get pub key:
  ```
  cat ~/.ssh/id_ed25519.pub 
  ```
