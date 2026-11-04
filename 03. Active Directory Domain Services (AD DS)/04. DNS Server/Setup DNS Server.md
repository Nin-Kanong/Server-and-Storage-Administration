<h1 align="center"> Setup DNS Server </h1>



---


#### Setup DNS:
Go to `Setting` -> `Network & Internet`:
<img width="1917" height="942" alt="image" src="https://github.com/user-attachments/assets/81f490c8-4014-4c3b-a35a-e9e1f7ea23fa" />

<img width="892" height="842" alt="image" src="https://github.com/user-attachments/assets/c346ca49-c26e-45d8-b594-9b429db54884" />

Input **DNS** like our server IP Address:
<img width="1177" height="876" alt="image" src="https://github.com/user-attachments/assets/21f64480-d582-46b3-836a-e9461f90b63d" />


<img width="877" height="822" alt="image" src="https://github.com/user-attachments/assets/58e38306-a5d0-44fc-a61c-b8c8c981849f" />

<img width="1917" height="890" alt="image" src="https://github.com/user-attachments/assets/5f3eae89-7ec6-4ff7-b183-b378b04d3bed" />

<img width="943" height="657" alt="image" src="https://github.com/user-attachments/assets/0a52ea4f-f6f2-45bf-8ab8-a93ddc5f59ac" />

After `Right-Click` on `cybersec.com` -> click on `New Host (A or AAA`:
<img width="1203" height="800" alt="image" src="https://github.com/user-attachments/assets/91b2ae68-4c9f-43ba-8c4d-41a92f96d119" />

````
www
````
````
192.168.17.10
````
<img width="427" height="472" alt="image" src="https://github.com/user-attachments/assets/ab565e04-2df4-47e8-ac37-36c5a62491a2" />

> `192.168.127.10` is my IP.

<img width="508" height="216" alt="image" src="https://github.com/user-attachments/assets/e8ed6bdc-30ff-42cf-a59e-9c913694ee78" />

<img width="433" height="475" alt="image" src="https://github.com/user-attachments/assets/c81a6273-ffc7-4ddc-a781-7cf9f4b1b8cb" />

Now we see `www`:
<img width="1077" height="570" alt="image" src="https://github.com/user-attachments/assets/d3a0121e-20a7-408c-8ac0-7388d1453e06" />

Now we finished.

#### Test connection:

Ping our hostname:
````
hostname
ping DC01-AD
````
<img width="771" height="450" alt="image" src="https://github.com/user-attachments/assets/bbc91c6c-660e-4dbd-bead-c5cf02d7e278" />

But also in this it show with `IPv6`.

Then change it:

`Right-Click` on `Internet` -> choose `Open Network & Internet ettings`:
<img width="1913" height="943" alt="image" src="https://github.com/user-attachments/assets/78c3c3f9-565a-484d-bebc-3c390b3b8195" />

<img width="1920" height="743" alt="image" src="https://github.com/user-attachments/assets/96b5579c-903e-4412-bd02-d7eac5aa048c" />

<img width="1030" height="727" alt="image" src="https://github.com/user-attachments/assets/d1361e24-cf71-4680-bf9d-4d065caa5ac6" />

After in `IPv6` set it to `Off`:
<img width="487" height="882" alt="image" src="https://github.com/user-attachments/assets/d0b47571-854a-461b-a09b-e08aaf407af7" />

<img width="492" height="852" alt="image" src="https://github.com/user-attachments/assets/d477e379-18c5-4e25-bfa4-514de68bcade" />

<img width="876" height="697" alt="image" src="https://github.com/user-attachments/assets/87e8ace7-92ea-4eae-8f1f-9e5cc4e971e5" />


After press `Windows + R` -> Type:
````
ncpa.cpl
````
<img width="478" height="302" alt="image" src="https://github.com/user-attachments/assets/f7513bb5-ddde-4341-bb3b-ba57069e1aad" />

<img width="1407" height="473" alt="image" src="https://github.com/user-attachments/assets/4a628beb-b194-4e1c-bca5-134c4787c006" />

Untick in this:
<img width="482" height="570" alt="image" src="https://github.com/user-attachments/assets/8963e3b2-e63f-4591-87c6-92a826f045a4" />

<img width="490" height="567" alt="image" src="https://github.com/user-attachments/assets/ebfb04be-a96c-4c8a-a992-8dd8358720fc" />

After test connect it again:
````
ping DC01-AD
````
<img width="587" height="355" alt="image" src="https://github.com/user-attachments/assets/702c4914-376a-4e45-8e87-a0b1a7b2858d" />

Now we see this, then `ping` to our domain:
````
ping cybersec.com
````
<img width="640" height="318" alt="image" src="https://github.com/user-attachments/assets/21469d80-42de-4f2c-b038-0d7e1608a263" />


Now we finished to create doman.

---


### Test Some connect & Join Domain:


#### Test some connection:
Go to our **Windows Client** -> press `Windows + R` -> type:
````
ncpa.cpl
````
<img width="402" height="206" alt="image" src="https://github.com/user-attachments/assets/e4f432ee-afaa-4920-9917-a0292edefa75" />

<img width="1116" height="461" alt="image" src="https://github.com/user-attachments/assets/4113eae8-1ab2-496f-a792-e82ad3839bac" />

`Doble-Click` on `Internet Protocol Version 4`:
<img width="363" height="466" alt="image" src="https://github.com/user-attachments/assets/f78f532d-666b-47e2-9715-59351097605f" />


After input the **DNS Server** ip of windows server:
````
192.168.127.10
````
<img width="402" height="456" alt="image" src="https://github.com/user-attachments/assets/2a1803c2-357b-4507-9910-3e7c203a7209" />

After click `Ok` -> then `Ok`:
<img width="366" height="471" alt="image" src="https://github.com/user-attachments/assets/0febdf30-412c-47d1-a6c5-d5bf9f034b95" />

> Note: `192.168.127.10` is my windows server IP.

Afte test connection to our **Windows Server**:
````
ping 192.168.17.10
````
````
ping cybersec.com
````
<img width="629" height="527" alt="image" src="https://github.com/user-attachments/assets/3ed9524e-2ce9-4611-8b15-d971006f1dc6" />

Now we got successful.

---
