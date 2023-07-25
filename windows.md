# Windows Instructions</br>

- ### [Installing `MSYS2`](#win_installing_msys2)</br>
- ### [Installing packages with pacman](#win_installing_packages)</br>
- ### [Installing git and GitHub CLI](#win_installing_git)</br>

---

</br>

<a name="win_installing_msys2"></a>

## Installing MSYS2

### Download installer
Download MSYS2 from [here](https://www.msys2.org). You should get an exe similar to this: `msys2-86_x64-20230718.exe`

### Install MSYS2
Run the exe and follow the instructions to install MSYS2 to a convenient directory like `C:/msys64`. Remember this directory as we will need it later.

### Adding MSYS2 to your PATH
After the install has completed, go to **Edit the system environment variables** which can be accessed from the start menu and add the following to your PATH system environment variable `<location\of\MSYS2>\ucrt64\bin` usually this is just `C:\msys64\ucrt64\bin`

<a name="win_installing_packages"></a>

## Installing GCC and CMake
Once MSYS2 has been installed and added to your PATH, open the MSYS2 bash and install all required packages using the following command:
```shell
pacman -Syu mingw-w64-ucrt-x86_64-{gcc,cmake}
```
Before moving on, verify that both packages have been installed properly by trying these commands in a normal terminal (eg: cmd.exe):
```shell
gcc --version
cmake --version
```
</br>
At this point, if you get an error about `gcc/cmake is not a recognized command`, double check your path is set correctly and then restart your terminal

<a name="win_installing_git"></a>

## Installing git

### Download `git`

Download git from [here](https://git-scm.com/download/win). You should get an exe similar to this: `Git-2.30.0.2-64-bit.exe`

<img src="images/win_images/git-01-download_git_00.png" alt="download_git" width="1000"/>

</br>

### Install `git`

Open/run the executable, and follow the steps to install. You can safely stick with the default options for everything to Install!

</br>

### Check git installation

To make sure git is installed correctly

```sh 
git --version
```

<img src="images/win_images/git-02-git_version.png" alt="download_git" width="1000"/>

<br/>

### Configure git

Configure git with username and email address:

```shell
git config --global user.name "stephengineer"
git config --global user.email swang03@pasadena.edu
```
### Download the GitHub CLI

The GitHub CLI can be downloaded from [here](https://github.com/cli/cli/releases/latest). Download the windows amd64 installer, you should download an msi file like: `gh_2.32.1_windows_amd64.msi`

### Install GitHub CLI

Open the .msi and click through to install the GitHub CLI 

### Login to GitHub

To login to GitHub

```shell
gh auth login
```

The CLI will step you through logging in with your github account

---

Once you have installed:
- **MSYS2**
- **GCC**
- **CMake**
- **git**
- **GitHub CLI**

you can move on to the [next step](start_project.md)
