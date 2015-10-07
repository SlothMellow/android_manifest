SlothMellow by Team Nocturnal
Download the source

Please read the building instructions before proceeding.

Initialize:

Create the build directory :

$ mkdir ~/dev
$ mkdir ~/dev/SlothMellow
$ cd ~/dev/SlothMellow
Init core trees without any device/kernel/vendor :

$ repo init -u https://github.com/SlothMellow/android_manifest.git -b sm6

now  sync the repo

$ repo sync

Building

After the sync is finished, please read the instructions from the Android site on how to build.

. build/envsetup.sh
brunch
make -j8
You can also build (and see how long it took) for specific devices like this:

. build/envsetup.sh
time lunch
make -j8
Remember to make clobber every now and then!
