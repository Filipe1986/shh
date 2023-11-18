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
Adding a second SSH

  ```
  ssh-keygen -t rsa -C "your_email@example.com"
  ```
  ```
  open ~/.ssh/config   
  ```
  Add
  ```
  Host XXXXXX.github.com
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.ssh/id_rsa
  ```


  Add key to git
  ```
  ssh-add -K ~/.ssh/id_rsa
  ```

  Test 
  ```
  ssh -T git@github.com
  ```

  Success Reponse
  Hi ______! You've successfully authenticated, but GitHub does not provide shell access.

