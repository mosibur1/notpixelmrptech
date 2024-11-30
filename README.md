## **CONFIGURE TERMUX**

After Installing Termux, Make Sure You Allowed Storage Permission On Termux (device app) Settings. Or Run This Command In Termux -
```
termux-setup-storage
```
**Install Python 3.10 -**
```
pkg update && upgrade
```
```
pkg install tur-repo
```
```
pkg install python-is-python3.10
```
```
pkg install -y rust binutils
```
```
CARGO_BUILD_TARGET="$(rustc -Vv | grep "host" | awk '{print $2}')" pip install maturin
```
# **GIT CLONE THE SCRIPT**
```
pkg install git
```
```
git clone https://github.com/ashtrobe/notpixel-ad.git
```
# **CHANGE DIRECTORY TO SCRIPT FOLDER**
```
cd notpixel-ad
```
# **INSTALL REQUIREMENTS**
```
pip install -r requirements.txt
```
```
pkg install patchelf
```
```
patchelf --add-needed libpython3.10.so.1.0 pyarmor_runtime_004817/android_aarch64/pyarmor_runtime.so
```
# **PASTE QUERY ID INSIDE ```query_ids.txt```**
```
pkg install nano
```
```
nano query_ids.txt
```
# **IF YOU WANNA USE PROXIES**
```
nano proxies.txt
```
# **RUN SCRIPT**
```
python main.py
```
