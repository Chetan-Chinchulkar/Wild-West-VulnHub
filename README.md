# Wild-West-VulnHub

Link : [https://www.vulnhub.com/entry/westwild-11,338/](https://www.vulnhub.com/entry/westwild-11,338/)

- Network → bridged adapter
- Get IP
    
    ```bash
    netdiscover
    ```
    
    Save in a file
    
    ```bash
    nmap -A -vv IP
    ```
    
    ```bash
    enum4linux IP
    smbclient -L //IP
    smbclient //IP/USER
    get FLAG.txt
    get avenge.txt
    ```
    
    for hashed code, 
    
    ```bash
    echo "HASH_CODE" | base64 -d
    ```
    
    ```bash
    ssh USER@IP
    ```
    
    ```bash
    sudo -l
    ```
    
    Use priviledge escalation
    
    ```bash
    find / -writable -type d 2>/dev/null
    ```
    
    ```bash
    check all the files
    ```
    
    ```bash
    su USER2
    sudo -l
    su
    sudo -i
    ```
