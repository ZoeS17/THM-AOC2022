### Day 7

<details>
<summary>1. What is the version of CyberChef found in the attached VM?</summary>

```9.49.0```<br><br>This is located in its own folder in our Downloads directory.
</deatils>
<details>
<summary>2. How many recipes were used to extract URLs from the malicious doc?</summary>

```10```<br><br>If we follow the steps in the walkthrough of the room we known these steps are: Add the file to CyberChef, Extract strings(minimum length of 258, all printable), remove `[\[\]_\n]` pattern, drop bytes(0-124), decode base64, decode-UTF16LE, find and remove the ``['()+'"`]``, find `]b2H_` and replace with `http`, extract URLs, split on `@`.
</deatils>
<details>
<summary>3. We found a URL that was downloading a suspicious file; what is the name of that malware?</summary>

```mysterygift.exe```<br><br>It's not often we download this type of file through a powershell script which is further hidden inside a word document.
</deatils>
<details>
<summary>4. What is the last defanged URL of the bandityeti domain found in the last step?</summary>

```hxxps[://]cdn[.]bandityeti[.]THM/files/index/```<br><br>You can add the `Defang URL` step to the end of your recipe to defang all the URLs and grab the last one with a `bandityeti` domain.
</deatils>
<details>
<summary>5. What is the ticket found in one of the domains? (Format: Domain/<GOLDEN_FLAG>)</summary>

```THM_MYSTERY_FLAG```<br><br>This should be the third URL extracted and the only one that fits the given format.
</deatils>
6. If you liked the investigation today, you might also enjoy the [Security Information and Event Management](https://tryhackme.com/module/security-information-event-management) module!
