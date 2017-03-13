Local manifests
===============
GT-N7100

This goes in .repo/local_manifests/roomservice.xml

Create snapshot
===============
repo manifest -o snapshot.xml -r

Restore snapshot
================
cp snapshot.xml .repo/manifests/
repo init -m snapshot.xml
repo sync -d
