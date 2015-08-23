English
==========

Android for MaxiCM Supported devices - CyanogenMod 11.0 [MaxiCM]
===========

Getting Started
---------------

To initialize your local repository using the MaxiCM trees, use a command like this:

    repo init -u git://github.com/MaxiCM/MaxiCM.git -b cm-11.0

Then to sync up:

    repo sync -j5
    
How to add local_manifest to download repo:

    cd .repo/manifests/local_manifest
    cp local_manifest.xml ../../
    cd ../../../
    repo sync -j5 

How to build to your Device (2 methods):

Normal Method:

    source build/envsetup.sh
    brunch (device codename)
    
New MaxiCM Vendor Method:

    ./MaxiCM-build.sh -c1 (device codename)

Flash ZIP:

    out/target/product/DEVICENAME/cm-VERSION-DEVICENAME.zip

Español
=========

Android para Dispositivos Soportados de MaxiCM- CyanogenMod 11.0 [MaxiCM]
=========

Empezando
------------

Para iniciar tu repositorio local usando el arbol de MaxiCM, una un comando como este:

    repo init -u git://github.com/MaxiCM/MaxiCM.git -b cm-11.0
    
Para sincronizar:

    repo sync -j6 -f
    
Como añadir el Local_manifest a tu repo de descarga:

    cd .repo/manifests/local_manifest
    cp local_manifest.xml ../../
    cd ../../../
    repo sync -j5
    
Como construir para tu dispositivo (2 metodos):

Metodo normal: 

    source build/envsetup.sh
    brunch (device codename)

Nuevo metodo vendor CM:

    ./MaxiCM-build.sh -c1 (device codename)
    
Flashea la ROM

    out/target/product/DEVICENAME/cm-VERSION-DEVICENAME.zip
