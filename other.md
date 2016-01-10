1,. solved this problem. Create a symbolik link named /usr/bin/java dan point it to /home/your_name/your_jdk_folder/bin/java

 This is the sample command in terminal/konsol

 sudo ln -s /home/azware/tmp/jdk1.7.0_03/bin/java /usr/bin/java
 link : http://stackoverflow.com/questions/11441928/linux-ubuntu-android-sdk-manager-not-starting-up-androidjava-not-found/17418841#17418841


2,'Cannot run program "/home/antz/Development/adt-bundle-linux/sdk/platform-tools/adb": error=2 No such file or directory' while attempting to get adb version from
 /home/antz/Development/adt-bundle-linux/sdk/platform-tools/adb


I'm using Ubuntu 14.04 LTS 64-bit and the following code works for me;

sudo apt-get install lib32z1 lib32z1-dev
sudo apt-get install lib32stdc++6

Summary:

After I tried apt-get install ia32-libs, but apt package tool suggest that;

Package ia32-libs is not available, but is referred to by another package.
This may mean that the package is missing, has been obsoleted, or is only available from another source.

However the following packages replace it:
  lib32z1 lib32ncurses5 lib32bz2-1.0

Then the above code works for me.
link: http://stackoverflow.com/questions/13571145/android-adb-not-found/13571288#13571288
