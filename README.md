# INSTALL-KALINET-HUNTER
This is only for educational purpose do not misuse it 
## Kali-Nethunter [non-root]:

[Kali NetHunter](https://www.kali.org/get-kali/#kali-mobile)) is a Mobile Penetration Testing Platform, and it allows for maximum flexibility with no commitment.

_For use on **unmodified stock Android phones without voiding the warranty**!_
the maker R.k.s-ahacker
## Screenshot:

![alt text](NH-Rootless-KeX.png)

## Prerequisite:

- Android Device (Stock unmodified device, no root or custom recovery required)

## Installation:

- Install the **NetHunter-Store app** from: <https://store.nethunter.com/>
- From the Kali NetHunter Store, install **Termux**, **NetHunter-KeX client**, and **Hacker's keyboard**
  _Note: The button "install" may not change to "installed" in the store client after installation - just ignore it. Starting termux for the first time may seem stuck while displaying "installing" on some devices - just hit enter._
- Open **Termux** and type:

<!-- https://offs.ec/2MceZWr -> https://raw.githubusercontent.com/popeye0013/kali-nethunter-project/main/install-nethunter-termux -->

## Setting Up Our Environment:

Next up, we would need some packages which we would need during the installation process.

First, update and upgrade the system with :
```
pkg update && pkg update -y
```

Next up we need to setup our system so that we can access the files created by Termux outside of our Termux session as well. This can be done with :
```
termux-setup-storage
```

Once you have granted the required Permissions, finally install the required packages with :
```
pkg install wget fish
```

Once done, we can proceed to the actual installation step.
Next we need to fetch and execute a script which will install Kali Linux for us. To fetch the script, type:
```
wget https://raw.githubusercontent.com/popeye0013/kali-nethunter-project/main/install-nethunter-termux
```

Now, we need to make the script executable and run it with:
```
chmod +x install-nethunter-termux
```
```
./install-nethunter-termux
```
This will fetch Kali Linux files and install them for us on our Android device. The script would fetch around 1.5GB of files so naturally, it might take a lot of time depending upon your network speed. Once the script is done extracting the rootfs file, you can even delete it.

Once the script has finished, you can run Kali Nethunter from the CLI.

To launch Kali Linux in CLI mode, type:
```
nethunter
```

This would drop into a shell on Kali Linux. You can now use Kali Tools or check your OS with
```
$ cat /etc/os-release | grep "\bNAME="
NAME="Kali GNU/Linux"
```
![alt text](nethunter.png)


## Usage:

Open Termux and type one of the following:

<!-- Make sure `./install-nethunter-termux` is in sync -->

| Command                   | To                                                      |
| ------------------------- | ------------------------------------------------------- |
| `nethunter`               | Start Kali NetHunter command line interface             |
| `nethunter kex passwd`    | Configure the KeX password (only needed before 1st use) |
| `nethunter kex &`         | Start Kali NetHunter Desktop Experience user sessions   |
| `nethunter kex stop`      | Stop Kali NetHunter Desktop Experience                  |
| `nethunter <command>`     | Run `<command>` in Kali NetHunter environment           |
| `nethunter -r`            | Start Kali NetHunter cli as root                        |
| `nethunter -r kex passwd` | Configure the KeX password for root                     |
| `nethunter -r kex &`      | Start Kali NetHunter Desktop Experience as root         |
| `nethunter -r kex stop`   | Stop Kali NetHunter Desktop Experience root sessions    |
| `nethunter -r kex kill`   | Kill all KeX sessions                                   |
| `nethunter -r <command>`  | Run `<command>` in Kali NetHunter environment as root   |

_Note: The command `nethunter` can be abbreviated to **`nh`**._

_Note: If you ran KeX in the background (`&`) **without having set a password**, you will need to bring it back to the foreground (i.e. via `fg <job id>`) then prompted to enter the password, finally you can then send it to the background again (via `Ctrl + z` and `bg <job id>`)_

To use KeX, start the KeX client, enter your password and click connect.

_Note: For a better viewing experience, enter a custom resolution under "Advanced Settings" in the KeX Client_

## Connect with us on:
<!-- 🌟 Optional Banner - यहां अपना बैनर लिंक लगाएं -->
<!-- ![Banner](https://your-banner-image-link.com/banner.jpg) -->

<p align="center">
  <a href="https://www.instagram.com/darklight000999_?igsh=cmEwN3htaTRodzl3">
    <img src="https://img.shields.io/badge/Instagram-%23E4405F.svg?style=for-the-badge&logo=instagram&logoColor=white" />
  </a>
  
  <a href="https://t.me/darklight000999">
    <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" />
  </a>
  
  <a href="https://chat.whatsapp.com/KALyrkZm2ru2xiTY9u0Tc0?mode=ac_t">
    <img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" />
  </a>
  
  <a href="https://www.facebook.com/darklight000999">
    <img src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white" />
  </a>
  
  <a href="https://youtube.com/@mr_br_hacker_33?si=IBcIbcrVE1Xur_vL">
    <img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" />
  </a>
  
  <a href="https://github.com/Darklight000999">
    <img src="https://img.shields.io/badge/GitHub-000000?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  
  <a href="https://share.google/BIo6sUsdFCFMMkc0z">
    <img src="https://img.shields.io/badge/Google%20Business-4285F4?style=for-the-badge&logo=google&logoColor=white" />
  </a>
</p>
