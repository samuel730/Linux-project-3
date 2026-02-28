## 2. Lab Environment

#### Host OS: Windows

#### Virtualization Tool: VirtualBox

#### VM Management Tool: Vagrant

#### Guest OS: Ubuntu 18.04 LTS

#### Package Manager: APT (Advanced Packaging Tool)
--- 
### 3. Procedure and Implementation

#### Step 1: Accessing the Linux System

Command used:
```
vagrant ssh
```
Expected output:
```
Welcome to Ubuntu 18.04.6 LTS (GNU/Linux 4.15.0-212-generic x86_64)
vagrant@ubuntu-bionic:~$
```
<img width="1857" height="1045" alt="Screenshot 2026-02-28 125842" src="https://github.com/user-attachments/assets/df235a29-cba4-4d0c-8f2a-3b6bd68b544d" />

#### Step 2: Updating Package Repositories
Command used:
```
sudo apt update
```
Observed output:
```
Hit:1 http://security.ubuntu.com/ubuntu bionic-security InRelease
Hit:2 http://archive.ubuntu.com/ubuntu bionic InRelease
Reading package lists... Done
17 packages can be upgraded.
```
<img width="1352" height="340" alt="Screenshot 2026-02-28 130110" src="https://github.com/user-attachments/assets/e0a45064-85ff-4d70-a5f1-771623e713d2" />

#### Step 3: Installing a Package (curl)
Command used:
```
sudo apt install curl -y
curl --version
```
Observed output:
```
curl 7.58.0 (x86_64-pc-linux-gnu) libcurl/7.58.0 OpenSSL/1.1.1 ...
Protocols: dict file ftp ftps gopher http https ...
```
<img width="2531" height="487" alt="Screenshot 2026-02-28 130411" src="https://github.com/user-attachments/assets/5382bc70-a96f-4554-a8df-61e53f183611" />

#### Step 4: Upgrading Installed Packages

Command used:
```
sudo apt upgrade -y
```
Observed output:
```
Calculating upgrade... Done
17 upgraded, 6 newly installed, 0 to remove, and 0 not upgraded.
...
Processing triggers for systemd (237-3ubuntu10.57) ...
```
<img width="1180" height="1377" alt="Screenshot 2026-02-28 130607" src="https://github.com/user-attachments/assets/5ed0f22b-9ee3-421e-867e-9f1c6437fa44" />

<img width="1326" height="1377" alt="Screenshot 2026-02-28 130630" src="https://github.com/user-attachments/assets/09715ce4-97bc-4d56-9d83-69bbb05afe8a" />

#### Step 5: Searching for Packages

Command used:
```
apt search "web server"
```
Observed output:
```
Sorting... Done
Full Text Search... Done
389-admin/bionic 1.1.46-2 amd64 389 Directory Administration Server
analog/bionic 2:6.0-22 amd64  web server log analyzer
...
```
<img width="1326" height="1377" alt="Screenshot 2026-02-28 130630" src="https://github.com/user-attachments/assets/812b8d83-a200-4a5c-9e91-e7ed8a36203d" />
<img width="800" height="1373" alt="Screenshot 2026-02-28 131229" src="https://github.com/user-attachments/assets/fde7793f-1b55-44a0-a745-c42d4c32e3e1" />
<img width="1013" height="1375" alt="Screenshot 2026-02-28 131214" src="https://github.com/user-attachments/assets/94e2c0e9-9f48-484c-b854-f8c45a6c3445" />
<img width="952" height="1371" alt="Screenshot 2026-02-28 131158" src="https://github.com/user-attachments/assets/453e6678-f8dd-4268-9ce8-ac3201ef27f7" />
<img width="801" height="1373" alt="Screenshot 2026-02-28 131142" src="https://github.com/user-attachments/assets/c45d8e3d-be29-4f13-8dcd-af963820f53a" />
<img width="875" height="1378" alt="Screenshot 2026-02-28 131128" src="https://github.com/user-attachments/assets/df2bf87d-3783-4ca4-bd2c-83e7ef9b3e41" />
<img width="838" height="1375" alt="Screenshot 2026-02-28 131106" src="https://github.com/user-attachments/assets/290ad630-8631-4ebf-a503-66ff11a60d09" />
<img width="823" height="1378" alt="Screenshot 2026-02-28 131047" src="https://github.com/user-attachments/assets/4ad2570c-4140-4e31-8810-ab9875f58d07" />
<img width="910" height="1369" alt="Screenshot 2026-02-28 131030" src="https://github.com/user-attachments/assets/d482bc0b-04a3-47d4-9913-f2c731bc18c1" />
<img width="906" height="1374" alt="Screenshot 2026-02-28 131015" src="https://github.com/user-attachments/assets/98d52c21-766d-4c88-aafe-6667d6e4e7e7" />

#### Step 6: Listing Installed Packages

Command used:
```
dpkg --list
```
Observed output (sample):
```
ii  curl         7.58.0-2ubuntu3.24   amd64  command line tool for transferring data with URL syntax
ii  apt          1.6.12               amd64  commandline package manager
```
<img width="2432" height="1379" alt="Screenshot 2026-02-28 131452" src="https://github.com/user-attachments/assets/7552859c-dca8-4062-9a52-227592fec6c1" />
<img width="2552" height="1373" alt="Screenshot 2026-02-28 131425" src="https://github.com/user-attachments/assets/ea90be77-f551-4c0d-87a4-dae7306090c8" />
<img width="2082" height="1367" alt="Screenshot 2026-02-28 131630" src="https://github.com/user-attachments/assets/7422ee43-f4b5-4d6a-802f-9ccb8f06b8e0" />
<img width="2221" height="1377" alt="Screenshot 2026-02-28 131606" src="https://github.com/user-attachments/assets/6503d5e2-d19f-403d-aeaf-0e9ff3c30fa3" />
<img width="2301" height="1375" alt="Screenshot 2026-02-28 131547" src="https://github.com/user-attachments/assets/828b3013-bd6f-4bf0-ae4a-442419e93a11" />
<img width="2216" height="1376" alt="Screenshot 2026-02-28 131521" src="https://github.com/user-attachments/assets/86a876c3-fdcf-4f2b-b88f-54d8d7697fa7" />

### 4. Challenges Encountered

During the lab, the following issues were encountered:

- Temporary DNS resolution failures when updating repositories.

- Network latency caused slow package downloads.

- Confusion about package manager commands between Debian/Ubuntu (apt) and Red Hat-based systems (yum/dnf).

These issues were resolved by:

- Configuring DNS in /etc/systemd/resolved.conf and restarting networking services.

- Patience while large upgrades downloaded.

- Carefully checking package manager syntax for the Ubuntu environment.

### 5. Conclusion

This lab provided practical experience in Linux package management. Through this exercise, I learned how to:

- Update package repositories to ensure access to the latest software.

- Install and remove packages using apt.

- Search for software packages by keywords.

- List installed packages to audit system software.

- Upgrade all installed packages to the latest versions.

- Troubleshoot common package management and network-related issues.

This lab successfully demonstrated how Linux system administrators manage software and maintain system security and stability.

### 6. Reflection / Learning Outcome

- I now understand the difference between apt, yum, and dnf package managers.

- I gained confidence in safely installing and removing packages without breaking system dependencies.

- I developed troubleshooting skills for network and repository issues.

- This lab reinforced the importance of keeping software updated to prevent vulnerabilities.

### 7. References

Canonical. (n.d.). Ubuntu documentation. https://help.ubuntu.com

Shotts, W. E. (2019). The Linux command line: A complete introduction. No Starch Press.








