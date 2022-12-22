### Day 21

First, if you don't already have a rtsp server go ahead and clone the suggested one off [github](https://github.com/aler9/rtsp-simple-server) or docker(`docker run --rm -it --network=host aler9/rtsp-simple-server
`). You'll also need [mosquitto](https://mosquitto.org/download/). While those download and install go ahead and read the challenge description until the `Practical Application`.

Secondly, let's start the Virtual Machine by pressing the `Start Machine` button at the top of this task. You may access the VM using the `AttackBox` or your VPN connection.

<details>
<summary>1. What port is Mosquitto running on? </summary>

```1883```
</details>
<details>
<summary>2. Is the device/init topic enumerated by Nmap during a script scan of all ports? (y/n)</summary>

```y```
</details>
<details>
<summary>3. What Mosquitto version is the device using?</summary>

```1.6.9```
</details>
<details>
<summary>4. What flag is obtained from viewing the RTSP stream?</summary>

```THM{UR_CAMERA_IS_MINE}```
</details>
5. If you want to learn more check out the [Command Injection](https://tryhackme.com/room/oscommandinjection) room or the [Vulnerability Research](https://tryhackme.com/module/vulnerability-research) module!
