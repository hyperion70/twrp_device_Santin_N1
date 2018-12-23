TWRP device tree for Santin N1 mt6757 (helio p25) || by hyperion70 - 2018

=================================

To recovery build in the Lineage OS 15.1 sources

	$ cd $(SOURCE)/bootable
    $ rm -rf recovery
    $ git clone https://github.com/omnirom/android_bootable_recovery -b android-8.1 recovery
    $ cd recovery

    $ git apply -v ../../device/leagoo/M8/twrp_recovery.patch
    $ cd ../..

	$ . build/envsetup.sh
    $ breakfast N1
	$ make clean
	$ make recoveryimage
