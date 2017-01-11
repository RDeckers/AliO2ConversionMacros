# AliO2ConversionMacros
Experimental conversion macro for creating new AoDs from old data for the ALICE's O2 upgrade.

## Pre-requisites

### Install the Aliroot/aliphysics branch for the O2 AOD developement

1. Init alibuild with a separate folder
   ```
   aliBuild init AliRoot,AliPhysics -z ali-aod-dev
   ```

2. Manually change the aliroot and aliphysics branch to the AOD developement branch
   ```bash
   $ cd ali-aod-dev/AliPhysics
   $ git checkout aod-upgrade
   $ cd ../AliRoot
   $ git checkout aod-upgrade
   ```

3. Complile
   ```
   $ aliBuild -j 2 -z -w ../sw build AliPhysics
   ```
### Install custom macros to produce the new AODs
