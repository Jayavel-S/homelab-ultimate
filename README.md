<h1 align="center" style="margin-top: 0px;">Ultimate Homelab Setup</h1>

<p align="center" >Shell based script to install Docker, and a set of different self-hostable applications compatible with Ubuntu/Debian based systems.</p>

## Prerequisites
  - You need to have an Ubuntu/Debian-based machine.
  - A good network connection to download the applications.
 
## Usage

Open Terminal (if using a desktop environment) or Putty/any SSH tool that you use (if using a server environment/headless machine) and connect to your instance. 

1. Download the script by running

```sh 
   wget https://raw.githubusercontent.com/Jayavel-S/homelab-ultimate/main/install.sh
```

<details><summary>Getting permission denied error?</summary>
<p>

Just add `sudo` in front.

```sh 
   sudo wget https://raw.githubusercontent.com/Jayavel-S/homelab-ultimate/main/install.sh
```

</p>
</details>

2. Now, you need to provide 'executable' permissions to it.
```sh 
   sudo chmod +x ./install.sh
```

3. Run the script
```sh 
   ./install.sh
```

## Features

1. Supports both AMD64 and ARM architectures with easy to follow instructions.
2. Grabs the latest version of Docker, Docker Compose (available in apt repo) and Portainer by default.
3. Skips the installation of Docker and Docker Compose if the system already has it installed.
4. Uses only FOSS (Free and Open Source Software) applications.
5. Includes database support (MySQL or MariaDB) for crucial applications.
6. Gives the ability to provide custom username and password along with desired directory/path mappings.
7. Takes the UID and GID by default (from the system) and applies it to the application's configuration.
8. Outputs all the information to a log file for reference or troubleshooting.
9. Provides the URL to access the application by taking note of the IP allocation to the system.
10. Detailed documentation and under active development.

## Packages

I have included some packages that lets you install and customize the applications to your needs. The available options are:

- Basic Setup
- Nextcloud Package
- Website Package
- Media Server Package
- General Apps

>Visit the **[documentation](https://github.com/Jayavel-S/homelab-ultimate/blob/main/docs/README.md)** section to know about the prompts and package specific instructions.

Once you make the selection, you might be asked additional questions that helps you tailor this installation to your needs. Make sure to read the prompts carefully and proceed with installation.

Choosing any option will get the default dependencies taken care of (i.e.) the script will install Docker, Docker-Compose and Portainer.

**[Back to Top](#ultimate-homelab-setup)**

## Changelog

<details><summary>Version 2.0</summary>
<p>

   - Added UI like support for getting user inputs using Whiptail.
   - Users can now just select the apps they want installed from the check list displayed.
   - Added Portainer check to see if Portainer is already installed.
   - Provided a selection menu for users to choose if they want to install Portainer or not.
   - Fixed the spinner! (previous version sometimes ended abruptly in some devices).

</p>
</details>

## Currently working on

   - A way to get user's input for assigning ports to the application during install.
   - Trying to make it compatible for other distros.
   - Making a separate file that houses all applications and can be invoked from the main script for ease of use.

### Legal Terms

Do note that there is no warranty provided with this script and it is completely open for everyone to provide contributions. This script is free to use in any private or a commercial deployment.

### Support

If you are facing any issues with using this script or if any of the applications are not getting installed properly, you can always create an issue through Github. Please make sure that you tried some basic troubleshooting steps prior to raising an issue here.


Thank you for visiting! 
**[Back to Top](#ultimate-homelab-setup)**
