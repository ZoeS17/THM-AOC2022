### Day 3

<details>
<summary>1. What is the name of the Registrar for the domain `santagift.shop`?</summary>

```Namecheap, Inc```<br><br>If we run `whois santagift.shop` and make sure to drop the tailing `.'` off the Registrar field in the response.
</details>
<details>
<summary>2. Find the website's source code (repository) on `github.com` and open the file containing sensitive credentials. Can you find the flag?</summary>

```{THM_OSINT_WORKS}```<br><br>As illuded to in the lead-up to our questions there are three good canidates for searching  on `github.com` itself to find the source repo we need: `SantaGiftShop`, `SantaGift`, and `SantaShop`. A likely canidate to check and something you should always look at if it appears is `config.php`
</details>
<details>
<summary>3. What is the name of the file containing passwords?</summary>

```config.php```<br><br>I kindof gave this one away in the reasoning for the last answer. This file likely contains passwords for databases and other server side settings.
</details>
<details>
<summary>4. </summary>What is the name of the QA server associated with the website?</summary>

```qa.santagift.shop```<br><br>We can find this in either `config.php` or helpfully the README.md that rendered on the repo's main page.
</details>
<details>
<summary>5. What is the DB_PASSWORD that is being reused between the QA and PROD environments?</summary>

```S@nta2022```If we look again in `config.php` we can can find this information.
</details>
6. Check out this [room](https://tryhackme.com/room/googledorking) if you'd like to learn more about Google Dorking!
