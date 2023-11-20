# ![logo](https://github.com/maksim-volkmann/42-project-badges/blob/main/badges/born2beroote.png?raw=true)<br>Born2beroot

$${\color{red}\text{Note: This guide was created using a Mac!}}$$

## Mandatory part

`You must choose as an operating system either the latest stable version of Debian (no testing/unstable), or the latest stable version of Rocky. Debian is highly recommended if you are new to system administration.`
In this example, we are going to use Debian because it's easier.

1. Download the `debian-xx.x.x-amd64-netinst.iso` file from [here](https://cdimage.debian.org/debian-cd/current/amd64/iso-cd/).


1. Create VM for your project inside the VirtualBox.
![install](./img/born2beroot_01.png)
2. Name your VM anything you want, and for the `Folder`: field, select the `goinfre` folder. It will automatically choose your user's folder. You have to do this because every student gets 10GB of memory on the server, and the goinfre folder uses local memory, which is necessary as we require more than 10GB. Leave `ISO Image` empty.<br>
![goinfre](./img/goinfre.png)
![select](./img/born2beroot_02.png)
3. Select 1GB of RAM (it should be enough)
![memory](./img/born2beroot_03.png)
4. Select 30.8 GB for the simple BONUS part where we are going to set up partitions, and leave the VDI as the hard disk type. And press `Finish`.
![memory](./img/born2beroot_04.png)
5. Settings -> Storage -> Controller (Empty) -> Optical drive -> Choose a disk file... Then select the debian.iso file you just downloaded and press OK.
![iso](./img/born2beroot_05.png)
6. After all that, you can finally start your virtual machine. You should also change the display size if you want to see anything.
![scale](./img/born2beroot_06.png)
7. Select "Install".
![install](./img/born2beroot_07.png)
8. Select your language.
![language](./img/born2beroot_08.png)
9. Select your location. If your location is not here, just select `other`, the continent and you will find it!
![location](./img/born2beroot_09.png)
10. This instruction is from subject.pdf file, so name your hostname accordingly.<br>
`The hostname of your virtual machine must be your login ending with 42 (e.g., wil42). You will have to modify this hostname during your evaluation.`
![hostname](./img/born2beroot_11.png)
11. Skip the domain name.
![domain_name](./img/born2beroot_12.png)
12. Choose your root password. Write it down, you will need it later!
![root_pass1](./img/born2beroot_13.png)
13. Re-enter your password.
![root_pass2](./img/born2beroot_14.png)
14. Now, you need to create an additional user, as suggested in the subject.pdf. This user should have the same username as your intra username, but this time without adding 42, unlike what we did with the hostname.<br>
`In addition to the root user, a user with your login as username has to be present.`
![admin_user](./img/born2beroot_15.png)
15. Create a password for the user you are setting up. For simplicity, you can use the same password as you did for the root.
![user_pass1](./img/born2beroot_16.png)
16. Re-enter the password.
![user_pass2](./img/born2beroot_17.png)



### Password policy:

Requirements from the subject:

* Password has to expire every 30 days.
* After changing the password, users are required to wait for a minimum of 2 days before making any further modifications.
* The user has to receive a warning message 7 days before their password expires.
* The password must be 10 characters long and include at least one uppercase letter, one lowercase letter, and one number. Additionally, it must not contain more than 3 consecutive identical characters.
* The password must not include the name of the user.
* The following rule does not apply to the root password: The password must have
at least 7 characters that are not part of the former password.
* Your root password has to comply with this policy.

For the first 3, we have to modify the `sudo nano /etc/login.defs`.

Change the Password aging controls:<br>
`PASS_MAX_DAYS - 30` (Maximum number of days a passowrd may be used.)<br>
`PASS_MIN_DAYS - 2` (Minimum number of days allowed between passowrd changes.)<br>
`PASS_WARN_AGE - 7` (Number of days warning given before a pasword expires.)<br>
`sudo reboot` to save changes.<br>

For other requrements we are using [pam_pwquality](https://manpages.debian.org/testing/libpam-pwquality/pam_pwquality.8.en.html).<br>
To install: `sudo apt-get install libpam-pwquality`<br>
To change settings: `sudo nano /etc/pam.d/common-password`<br>
Line to eddit: `password 			requisite					pam_pwquality.so retry=3`<br>
Change to: `password requisite pam_pwquality.so retry=3 minlen=10 ucredit=-1 dcredit=-1 maxrepeat=3 reject_username difok=7 enforce_for_root`<br>


