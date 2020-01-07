BootStrap: debootstrap
OSVersion: xenial
MirrorURL: http://us.archive.ubuntu.com/ubuntu/
IncludeCmd: yes
Include: bash vim less man-db apt-utils tzdata

%setup

%environment

$post
  # Most from chpc ubuntu build def
  mkdir /uufs
  mkdir /scratch

%runscript

%test

%help
