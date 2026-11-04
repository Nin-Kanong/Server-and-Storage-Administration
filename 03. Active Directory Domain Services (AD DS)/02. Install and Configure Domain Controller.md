<h1 align="center"> Install and Configure Domain Controller </h1>


---


### Create Domain

Go to `Windows Server` -> `Server Manager`:
<img width="1920" height="943" alt="image" src="https://github.com/user-attachments/assets/8123b18f-023f-48aa-bd19-978a76f05810" />

<img width="982" height="692" alt="image" src="https://github.com/user-attachments/assets/aa96b446-0b28-46b2-8819-00db838aa7ea" />

<img width="983" height="696" alt="image" src="https://github.com/user-attachments/assets/9c29c978-38af-405c-b9d7-b2a34f9179b5" />

<img width="985" height="697" alt="image" src="https://github.com/user-attachments/assets/57cd7f34-46e0-465d-8daa-7058a1d085e5" />


After click on `Active Directory Domain Service`:
<img width="978" height="702" alt="image" src="https://github.com/user-attachments/assets/fbe78d4d-368b-4c11-b966-eeb9ab99223b" />

<img width="521" height="546" alt="image" src="https://github.com/user-attachments/assets/1667c2ee-82da-4f47-8032-c93209eff9a8" />

<img width="981" height="697" alt="image" src="https://github.com/user-attachments/assets/01a22cd0-a0cd-4843-8b54-c0ef3e0a5927" />

<img width="982" height="695" alt="image" src="https://github.com/user-attachments/assets/06c73610-4753-4acb-9292-1672c6763fc6" />

<img width="982" height="698" alt="image" src="https://github.com/user-attachments/assets/d2b032b3-5663-49c9-b383-f57c0ad0f9d1" />

<img width="981" height="693" alt="image" src="https://github.com/user-attachments/assets/1eff1111-fbaf-4502-8e99-1d07429902f2" />

After wait a few minute:
<img width="981" height="698" alt="image" src="https://github.com/user-attachments/assets/0f4b68b4-d51b-4535-8ad2-eecc2f431f9e" />


<img width="978" height="693" alt="image" src="https://github.com/user-attachments/assets/8a9fa994-1a13-429e-8090-b517c8827208" />

In this I use domain:
````
cybersec.com
````
<img width="957" height="705" alt="image" src="https://github.com/user-attachments/assets/80bcfc26-a079-4d0e-9f45-8caad0c52f64" />

<img width="956" height="698" alt="image" src="https://github.com/user-attachments/assets/6183381b-5352-4c69-86d5-6b690bba967a" />

In this why we see:
- **Forest functional level**: ``Windows Server 2016``
- **Domain functional level**: ``Windows Server 2016``

Cause The AD DS wizard showing Windows Server 2016 is the Active Directory Functional Level, not the OS version.

<img width="952" height="697" alt="image" src="https://github.com/user-attachments/assets/b9f1a399-3715-459c-98aa-5c1bf85d27ec" />

<img width="952" height="697" alt="image" src="https://github.com/user-attachments/assets/39011182-e055-4cec-b016-aeaeb7a64410" />

<img width="950" height="697" alt="image" src="https://github.com/user-attachments/assets/6102dc75-876c-4068-928e-92274f89082b" />

<img width="951" height="698" alt="image" src="https://github.com/user-attachments/assets/ebdbea09-c69a-4dec-a2b2-0b1d837b749a" />

<img width="952" height="706" alt="image" src="https://github.com/user-attachments/assets/6dfeca7b-70f3-44ee-b6c1-791ebf9b1107" />

After wait a few minute it will Restart auto:
<img width="1607" height="701" alt="image" src="https://github.com/user-attachments/assets/6fc04beb-8101-4f30-b34b-f969019afa64" />

After it finishe to restart and we will see our domin:
<img width="1912" height="995" alt="image" src="https://github.com/user-attachments/assets/58e686f6-4537-4f2c-b174-cc935fa310ed" />


Afte we login into our server then open our `Server Manager`:
<img width="1919" height="942" alt="image" src="https://github.com/user-attachments/assets/19dbfa26-c46b-4cbb-8d96-a09737d89404" />

Now we see our domain:
<img width="943" height="511" alt="image" src="https://github.com/user-attachments/assets/5a56d4ba-551f-46a5-aa0d-75d63de8d166" />

##### Explain:
| Folder/Object                 | What it is                         | Purpose                                    | Example Use                         |
| ----------------------------- | ---------------------------------- | ------------------------------------------ | ----------------------------------- |
| **cybersec.com (Domain)**     | Your Active Directory domain       | Main container for all AD objects          | Manage company users, PCs, policies |
| **Builtin**                   | Default built-in security groups   | Contains Windows default groups            | Administrators, Users, Guests       |
| **Computers**                 | Default computer container         | Stores computers joined to domain          | PC01, HR-PC, Client01               |
| **Domain Controllers**        | Contains Domain Controller servers | Stores DC machines                         | DC01-AD                             |
| **ForeignSecurityPrincipals** | External security identities       | Used for users/groups from trusted domains | Another domain user access          |
| **Managed Service Accounts**  | Service accounts managed by AD     | Runs services securely                     | IIS service, SQL service            |
| **Users**                     | Default user container             | Stores user accounts and groups            | Admin, John, HR user                |
| **Saved Queries**             | Custom searches                    | Quickly find objects                       | Find all disabled users             |


##### Important objects in AD

| Object            | Meaning                    |
| ----------------- | -------------------------- |
| User              | Person account             |
| Computer          | Joined machine             |
| Group             | Permission collection      |
| OU                | Folder to organize objects |
| Domain            | Company identity           |
| Domain Controller | Server that manages AD     |


In this we can check also in this our Computers (OU) hs no user join domn yet, and in Domain Controllers is `DC01-AD`:
<img width="935" height="636" alt="image" src="https://github.com/user-attachments/assets/253a6e5c-f6e4-40ca-a8c6-196aa1a22143" />


----
