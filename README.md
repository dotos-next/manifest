# DotOS 4.x - Android 10



Getting Started:
==============

To get started with the building process, you'll need to get familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

To initialize your local repository, use a command like this:

```bash
    repo init -u git://github.com/DotOS-next/manifest.git -b dot10
```

Then to sync up:
================

```bash
    repo sync -c -jx --force-sync --no-clone-bundle --no-tags
```

Additionally, you can define the number of parallel download repo should do:

```bash
    repo sync -f -jX --force-sync --no-clone-bundle --no-tags ( X is the number of parallel download repo should do choose depending on your cpu )
```

Compilation of Dot OS:
====================

From root directory of Project, perform following commands in terminal


```bash
source build/envsetup.sh
lunch dot_<devicecodename>-userdebug
make bacon
```
-----------------------------------------------------------------------------

• Submit your All patches through our [**Gerrit Code Review**](https://review.droidontime.com)

• Help us on translation through our [**Crowdin**](https://translations.droidontime.com)
