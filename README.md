# HOW TO INSTALL WSL for Windows 10 (also works on W11)

## 1 STEP
```
On the Windows 10 search bar search for 'Microsoft Store' and open it.
```
![1](./images/ms_store_app.png)
## 2 STEP
```
Search for "Windows Subsystem for Linux" and click on "Install"
```
## 3 STEP
![2](./images/ms_store_wsl.png)
```
On the Windows 10 search bar search for 'Windows Features' and open it.
```
## 4 STEP
![3](./images/features_win10.png)
```
Enable 2 features:
- Windows Subsystem for Linux
- Virtual Machine Platform
```
## 4 STEP
![4](./images/enabled_features.png)
```
Click on install, wait and restart the PC
```
## 5 STEP
![5](./images/installed_features.png)
```
Open the Windows Terminal (cmd) and check if WSL is installed correctly by executing:
wsl -v
```
## 6 STEP
![6](./images/check_wsl.png)
```
Check for all possible installations by executing:
wsl --list --online
```
## 7 STEP
![7](./images/list_wsl_os.png)
```
Install your favorite OS by executing:
wsl --install -d {OS}
```
## 8 STEP
![8](./images/install_os_wsl.png)
```
On the Windows 10 search bar search for 'WSL' and open it.
```
## 9 STEP
![9](./images/open_wsl.png)
```
Check if all it's OK
```
## 10 STEP
![10](./images/check_os_wsl.png)


# ERR 1
```
Sometimes with the basic user you don't have enough permissions to execute the 'ping' command.
You may execute:
sudo setcap cap_net_raw+ep /bin/ping
```
![11](./images/solved_ping.png)