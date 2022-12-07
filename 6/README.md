### Day 6

<details>
<summary>1. What is the email address of the sender?</summary>
```chief.elf@santaclaus.thm```<br><br>
</details>
<details>
<summary>2. What is the return address?</summary>
```murphy.evident@bandityeti.thm```<br><br>
</details>
<details>
<summary>3. On whose behalf was the email sent?</summary>
```Chief Elf```<br><br>
</details>
<details>
<summary>4. What is the X-spam score?</summary>
```3```<br><br>
</details>
<details>
<summary>5. What is hidden in the value of the Message-ID field?</summary>
```AoC2022_Email_Analysis```<br><br>
</details>
<details>
<summary>6. Visit the email reputation check website provided in the task. What is the reputation result of the sender's email address?</summary>
```RISKY```<br><br>
</details>
<details>
<summary>7. Check the attachments. What is the filename of the attachment?</summary>
```Division_of_labour-Load_share_plan.doc```<br><br>
</details>
<details>
<summary>8. What is the hash value of the attachment?</summary>
```0827bb9a2e7c0628b82256759f0f888ca1abd6a2d903acdb8e44aca6a1a03467```<br><br>Here we can extract the document without loading it into an email client like Thunderbird if we grab all the lines after the one begining `Content-Disposition: attachment; filename="Division_of_labour-Load_share_plan.doc"`(line #40 in the attackbox) and before `-----------------------03edd9c682a0c8f60d54b9e4bb86659f--`(line #1058) and save it into a file called `attachment.doc.b64` on the Desktop. We have to fix the data a bit so we can load up a terminal and `cd` into the `Desktop` then type open vim with `vim attachment.doc.b64`. We then want to put all of this on one line so we can type `:%s/\n//g` and then press enter to get it to replace all of the new-lines with nothing. Then we can save and quit by typing `:wq`. Now that we're back on the terminal type `cat attachment.doc.b64 | base64 -d > attachment.doc`. And finally we can get the sha256 hash of the actual attachment with `sha256sum attachment.doc`
</details>
<details>
<summary>9. Visit the Virus Total website and use the hash value to search. Navigate to the behaviour section. What is the second tactic marked in the Mitre ATT&CK section?</summary>
```defense evasion```<br><br>
</details>
<details>
<summary>10. Visit the InQuest website and use the hash value to search. What is the subcategory of the file?</summary>
```macro_hunter```<br><br>
</details>
11. If you want to learn more about phishing and analysing emails, check out the [Phishing](https://tryhackme.com/module/phishing) module!
