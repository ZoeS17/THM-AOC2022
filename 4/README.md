### Day 4

<details>
<summary>1. What is the name of the HTTP server running on the remote host?</summary>

```Apache```<br><br> In the output of `nikto -host $MACHINE_IP:80` the `Server` field gives us our answer.
</details>

<details>
<summary>2. What is the name of the service running on port 22 on the QA server?</summary>

```ssh```<br><br>
To find this out try running:```bash
nmap -sS $MACHINE_IP
```
</details>
<details>
<summary>3. What flag can you find after successfully accessing the Samba service?</summary>

```{THM_SANTA_SMB_SERVER}```<br><br> Check out the `flag.txt` file in the `admins` share.
</details>
<details>
<summary>4. What is the password for the username santahr?</summary>

```santa25```<br><br> Check out the `userlist.txt` file in the `admins` share.
</details>
5. If you want to learn more scanning techniques, we have a module dedicated to [Nmap](https://tryhackme.com/module/nmap)!
