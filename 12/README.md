### Day 12

<details>
<summary>1. What is the architecture of the malware sample? (32-bit/64-bit)</summary>

```64-bit```
</details>
<details>
<summary>2. What is the packer used in the malware sample? (format: lowercase)</summary>

```upx```
</details>
<details>
<summary>3. What is the compiler used to build the malware sample? (format: lowercase)</summary>

```nim```
</details>
<details>
<summary>4. How many MITRE ATT&CK techniques have been discovered attributed to the DISCOVERY tactic?</summary>

```2```
</details>
<details>
<summary>5. What is the registry key abused by the malware?</summary>

```HKCU\Software\Microsoft\Windows\CurrentVersion\Run```
</details>
<details>
<summary>6. What is the value written on the registry key based on the previous question?</summary>

```C:\Users\Administrator\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup\wishes.bat```
</details>
<details>
<summary>7. What are the names of two files created by the malware under the C:\Users\Administrator\ directory? (format: file1,file2 in alphabetical order)</summary>

```test.jpg,wishes.bat```
</details>
<details>
<summary>8. What are the two domains wherein malware has initiated a network connection? (format: domain1,domain2 in alphabetical order)</summary>

```bestfestivalcompany.thm,virustotal.com```
</details>
<details>
<summary>9. Going back to strings inside the malware sample, what is the complete URL used to download the file hosted in the first domain accessed by the malware?</summary>

```http://bestfestivalcompany.thm/favicon.ico```<br><br>My command prompt's scroll buffer was filled even with strings set to 30 characters(`strings -n 30 mysterygift.exe`) so I piped it to an out-file like this: `strings -n 30 mysterygift.exe > out.txt` and then used notepad's find to look for http.
</details>
10. If you enjoyed malware analysis, try the [Intro to Malware Analysis](https://tryhackme.com/room/intromalwareanalysis) or [Dissecting PE Headers](https://tryhackme.com/room/dissectingpeheaders) rooms next!
