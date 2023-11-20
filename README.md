# ![logo](https://github.com/maksim-volkmann/42-project-badges/blob/main/badges/born2beroote.png?raw=true)<br>Born2beroot

$${\color{red}\text{Note: This guide was created using a Mac!}}$$

## Mandatory part

`You must choose as an operating system either the latest stable version of Debian (no testing/unstable), or the latest stable version of Rocky. Debian is highly recommended if you are new to system administration.`
In this example, we are going to use Debian because it's easier.

1. Download the `debian-xx.x.x-amd64-netinst.iso` file from [here](https://cdimage.debian.org/debian-cd/current/amd64/iso-cd/).


1. Create VM for your project inside the VirtualBox.
![install](./img/born2beroot_01.png)
2. Name your VM anything you want, and for the `Folder`: field, select the `goinfre` folder. It will automatically choose your user's folder. You have to do this because every student gets 10GB of memory on the server, and the goinfre folder uses local memory, which is necessary as we require more than 10GB. Leave `ISO Image` empty.<br>
![select](./img/born2beroot_02_f.png)
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

![partition_selection](./img/partition_01.png)
![partition_selection](./img/partition_02.png)
![partition_selection](./img/partition_03.png)
![partition_selection](./img/partition_04.png)
![partition_selection](./img/partition_05.png)
![partition_selection](./img/partition_06.png)
![partition_selection](./img/partition_07.png)
![partition_selection](./img/partition_08.png)
![partition_selection](./img/partition_09.png)
![partition_selection](./img/partition_10.png)
![partition_selection](./img/partition_11.png)
![partition_selection](./img/partition_12.png)
![partition_selection](./img/partition_13.png)
![partition_selection](./img/partition_14.png)
![partition_selection](./img/partition_15.png)
![partition_selection](./img/partition_16.png)
![partition_selection](./img/partition_17.png)
![partition_selection](./img/partition_18.png)
![partition_selection](./img/partition_19.png)
![partition_selection](./img/partition_20.png)
![partition_selection](./img/partition_21.png)
![partition_selection](./img/partition_22.png)
![partition_selection](./img/partition_23.png)
![partition_selection](./img/partition_24.png)
![partition_selection](./img/partition_25.png)
![partition_selection](./img/partition_26.png)
![partition_selection](./img/partition_27.png)
![partition_selection](./img/partition_28.png)
![partition_selection](./img/partition_29.png)
![partition_selection](./img/partition_30.png)
![partition_selection](./img/partition_31.png)
![partition_selection](./img/partition_32.png)
![partition_selection](./img/partition_33.png)
![partition_selection](./img/partition_34.png)
![partition_selection](./img/partition_35.png)
![partition_selection](./img/partition_36.png)
![partition_selection](./img/partition_37.png)
![partition_selection](./img/partition_38.png)
![partition_selection](./img/partition_39.png)
![partition_selection](./img/partition_40.png)
![partition_selection](./img/partition_41.png)
![partition_selection](./img/partition_42.png)
![partition_selection](./img/partition_43.png)
![partition_selection](./img/partition_44.png)
![partition_selection](./img/partition_45.png)
![partition_selection](./img/partition_46.png)
![partition_selection](./img/partition_47.png)
![partition_selection](./img/partition_48.png)
![partition_selection](./img/partition_49.png)
![partition_selection](./img/partition_50.png)
![partition_selection](./img/partition_51.png)
![partition_selection](./img/partition_52.png)
![partition_selection](./img/partition_53.png)
![partition_selection](./img/partition_54.png)
![partition_selection](./img/partition_55.png)
![partition_selection](./img/partition_56.png)
![partition_selection](./img/partition_57.png)
![partition_selection](./img/partition_58.png)
![partition_selection](./img/partition_59.png)
![partition_selection](./img/partition_60.png)
![partition_selection](./img/partition_61.png)
![partition_selection](./img/partition_62.png)
![partition_selection](./img/partition_62_1.png)
![partition_selection](./img/partition_63.png)
![partition_selection](./img/partition_64.png)
![partition_selection](./img/partition_65.png)
![partition_selection](./img/partition_66.png)
![partition_selection](./img/partition_67.png)
![partition_selection](./img/partition_68.png)
![partition_selection](./img/partition_69.png)
![partition_selection](./img/partition_70.png)
![partition_selection](./img/partition_71.png)
![partition_selection](./img/partition_72.png)
![partition_selection](./img/partition_73.png)
![partition_selection](./img/partition_74.png)
![partition_selection](./img/partition_75.png)
![partition_selection](./img/partition_76.png)
![partition_selection](./img/partition_77.png)
![partition_selection](./img/partition_78.png)
![partition_selection](./img/partition_79.png)
![partition_selection](./img/partition_80.png)
![partition_selection](./img/partition_81.png)
![partition_selection](./img/partition_82.png)
![partition_selection](./img/partition_83.png)
![partition_selection](./img/partition_84.png)
![partition_selection](./img/partition_85.png)
![partition_selection](./img/partition_86.png)
![partition_selection](./img/partition_87.png)
![partition_selection](./img/partition_88.png)
![partition_selection](./img/partition_89.png)
![partition_selection](./img/partition_90.png)
![partition_selection](./img/partition_91.png)
![partition_selection](./img/partition_92.png)
![partition_selection](./img/partition_93.png)
![partition_selection](./img/partition_94.png)
![partition_selection](./img/partition_95.png)
![partition_selection](./img/partition_96.png)
![partition_selection](./img/partition_97.png)
![partition_selection](./img/partition_98.png)
![partition_selection](./img/partition_99.png)
![partition_selection](./img/partition_100.png)



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


