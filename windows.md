# Windows Instructions</br>

- ### [Installing `git`](#win_installing_git)</br>
- ### [Installing `cmake`](#win_installing_cmake)</br>
- ### [Installing `MinGW`](#win_installing_mingw)</br>

---

</br>

<a name="win_installing_git"></a>

## Installing git

</br>

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
$ git --version
```

<img src="images/win_images/git-02-git_version.png" alt="download_git" width="1000"/>

<br/>

### Login git

Login git with username and email address:

```sh
$ git config --global user.name "stephengineer"
$ git config --global user.email swang03@pasadena.edu
```

---

</br>

<a name="win_installing_cmake"></a>

## Installing cmake

</br>

### Download `cmake`

Download cmake from [here](https://cmake.org/download/). Choose the Windows win64-x64 Installer. You should get an msi with a name similar to this: `cmake-3.19.4-win64-x64.msi`

<img src="images/win_images/cm-00-download_site.png" alt="download_cmake" width="1000"/>

</br>

### Install `cmake`

Open/Run the executable file, and follow the steps to install.

<img src="images/win_images/cm-01-download_00.png" alt="install_cmake" width="1000"/>

</br>

Check I accept the terms in the License Agreement.

<img src="images/win_images/cm-01-download_01.png" alt="install_cmake" width="1000"/>

</br>

**Make sure** to select Add CMake to the system PATH for all users. You can create a Desktop icon if you want, but you will not need to use it for this class.

<img src="images/win_images/cm-01-download_03.png" alt="install_cmake" width="1000"/>

</br>

The default install location should be C:\Program Files\CMake\

> <img src="images/win_images/cm-01-download_04.png" alt="install_cmake" width="1000"/>

</br>

Install!

<img src="images/win_images/cm-01-download_05.png" alt="install_cmake" width="300"/>

<img src="images/win_images/cm-01-download_06.png" alt="install_cmake" width="300"/>

</br>

When it is done installing, click Finish.

<img src="images/win_images/cm-01-download_07.png" alt="install_cmake" width="1000"/>

</br>

### Check the version of the git again:

Let's check to see if `cmake` is installed successfully:

```sh
$ cmake --version
```

<img src="images/win_images/cm-02-cmake_version.png" alt="cmake_version" width="1000"/>

---

</br>

<a name="win_installing_mingw"></a>

## Install MinGW

</br>

### Is `MinGW` installed?

Let's check to see if `g++` is installed on your system:

```sh
$ g++ --version
```

If you do not get a response similar to this, then you do not have `g++` and/or `MinGW` on your system and you have to install it.

<img src="images/win_images/g++-00-g++_version.png" alt="g++_version" width="1000"/>

</br>

### Download `MinGW`

Download cmake from [here](https://sourceforge.net/projects/mingw/files/). You should get an exe named similar to this: `mingw-get-setup.exe`

</br>

### Install `MinGW`/`g++`

Open/Run the executable file, and follow the steps to install.

<img src="images/win_images/g++-01-download_00.png" alt="g++_install" width="300"/>

<img src="images/win_images/g++-01-download_01.png" alt="g++_install" width="300"/>

</br>

The default Installation location should be `C:/MinGW`. Once again, you can add a Desktop shortcut, but it will not be necessary for this class.

<img src="images/win_images/g++-01-download_02.png" alt="g++_install" width="1000"/>

</br>

If you get a warning that MinGW is already installed, you can either reinstall and continue with this walk through or choose `Run Now` and skip to the steps below with the MinGW Install Manager.

<img src="images/win_images/g++-01-download_03.png" alt="g++_install" width="1000"/>

</br>

Installing...

<img src="images/win_images/g++-01-download_04.png" alt="g++_install" width="1000"/>

</br>

When it is done installing, click Continue.

<img src="images/win_images/g++-01-download_06.png" alt="g++_install" width="1000"/>

</br>

The **MinGW Installation Manager** should be opened up automatically. For this class, you will need mingw32-base, mingw-gcc-g++, and mingw23-gcc-objc.

<img src="images/win_images/g++-02-selection_00.png" alt="g++_install" width="1000"/>

</br>

To select a package for installation, right click on it in the menu and select Mark for Installation.

<img src="images/win_images/g++-02-selection_01.png" alt="g++_install" width="1000"/>

</br>

Marked packages will be selected like this:

<img src="images/win_images/g++-02-selection_02_zoom.png" alt="g++_install" width="1000"/>

</br>

You **also** need to select the pthreads package from under <br/>
All Packages -> MinGW Libraries

<img src="images/win_images/99-01-pthread.png" alt="g++_install" width="1000"/>

</br>

Once all necessary packages have been marked, go to Installations > Apply Changes to install.

<img src="images/win_images/g++-02-selection_03.png" alt="g++_install" width="1000"/>

</br>

Click Apply

<img src="images/win_images/g++-02-selection_04.png" alt="g++_install" width="1000"/>

</br>

Once the changes are applied you may close the Installation Manager.

<img src="images/win_images/g++-02-selection_07.png" alt="g++_install" width="1000"/>

</br>

### Add g++ as a System Variable and to your path

Search for "path" in the task bar search box. Open Edit the system environment variables.

<img src="images/win_images/g++-03-path_00.png" alt="g++_path" width="600"/>

</br>

Click on "Environment Variables..."

<img src="images/win_images/g++-03-path_01.png" alt="g++_path" width="600"/>

</br>

Add the path to the gcc and g++ executables to environment variables as shown below and press OK.

<img src="images/win_images/g++-03-path_02.png" alt="g++_path" width="600"/>

</br>

Next, double click on the **user variable** Path (in the top half of the window). A window like this should pop up:

<img src="images/win_images/g++-03-path_before.png" alt="g++_path" width="600"/>

</br>

Click New, and enter `C:\MinGW\bin` to the text box. Click OK.

<img src="images/win_images/g++-03-path_after.png" alt="g++_path" width="400"/>

</br>

Your environment and user variables should look like this after you are done:

<img src="images/win_images/g++-03-path_03.png" alt="g++_path" width="400"/>

</br>

### Check the version of the g++ again:

To make sure `MinGW`/`g++` is installed correctly, if the version output doesn't show, reboot your machine and try again.

```sh
$ g++ --version
```

<img src="images/win_images/g++-00-g++_version.png" alt="g++_path" width="1000"/>

---

Once everything is installed, you can move on to the [next step](start_project.md)
