Installation
---

## Quick Cabal Method

Following  
https://github.com/jgm/pandoc/blob/master/INSTALL.md#quick-cabal-method
```
sudo apt-get install haskell-platform #takes 2-5min
cabal update
cabal install pandoc-crossref
```
** it takes about  an hour to do the installation

add in `.bashrc` the following line
```
##################################
# Setting PATH for pandoc binaries
export PATH=$HOME/.cabal/bin:$PATH
```


## issues

if your installation fails becaouse of networks connections. or
starting the installation after rebooting your machine
Try nuking ~/.ghc and ~/.cabal and starting again.
[ref](https://github.com/haskell/cabal/issues/4484)



## terminal output

$ sudo apt-get install haskell-platform
```

Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following packages were automatically installed and are no longer required:
  gnuplot5-data gnuplot5-qt libwxbase3.0-0v5 libwxgtk3.0-0v5 linux-headers-4.15.0-29 linux-headers-4.15.0-29-generic linux-headers-4.15.0-33
  linux-headers-4.15.0-33-generic linux-headers-4.15.0-34 linux-headers-4.15.0-34-generic linux-headers-4.15.0-36 linux-headers-4.15.0-36-generic
  linux-image-4.15.0-29-generic linux-image-4.15.0-33-generic linux-image-4.15.0-34-generic linux-image-4.15.0-36-generic linux-modules-4.15.0-29-generic
  linux-modules-4.15.0-33-generic linux-modules-4.15.0-34-generic linux-modules-4.15.0-36-generic linux-modules-extra-4.15.0-29-generic
  linux-modules-extra-4.15.0-33-generic linux-modules-extra-4.15.0-34-generic linux-modules-extra-4.15.0-36-generic
Use 'sudo apt autoremove' to remove them.
The following additional packages will be installed:
  alex cabal-install ghc happy hscolour libbsd-dev libghc-async-dev libghc-attoparsec-dev libghc-case-insensitive-dev libghc-fgl-dev libghc-gluraw-dev libghc-glut-dev
  libghc-hashable-dev libghc-haskell-src-dev libghc-html-dev libghc-http-dev libghc-hunit-dev libghc-mtl-dev libghc-network-dev libghc-network-uri-dev
  libghc-objectname-dev libghc-old-locale-dev libghc-old-time-dev libghc-opengl-dev libghc-openglraw-dev libghc-parallel-dev libghc-parsec3-dev libghc-primitive-dev
  libghc-quickcheck2-dev libghc-random-dev libghc-regex-base-dev libghc-regex-compat-dev libghc-regex-posix-dev libghc-scientific-dev libghc-split-dev libghc-statevar-dev
  libghc-stm-dev libghc-syb-dev libghc-text-dev libghc-tf-random-dev libghc-unordered-containers-dev libghc-vector-dev libghc-zlib-dev libxi-dev libxmu-dev libxmu-headers
Suggested packages:
  ghc-prof ghc-doc haskell-doc llvm-3.5 haskell-platform-doc haskell-platform-prof libghc-async-doc libghc-async-prof libghc-attoparsec-doc libghc-attoparsec-prof
  libghc-case-insensitive-doc libghc-case-insensitive-prof libghc-fgl-doc libghc-fgl-prof libghc-gluraw-doc libghc-gluraw-prof libghc-glut-doc libghc-glut-prof
  libghc-hashable-doc libghc-hashable-prof libghc-haskell-src-doc libghc-haskell-src-prof libghc-html-doc libghc-html-prof libghc-http-doc libghc-http-prof
  libghc-hunit-doc libghc-hunit-prof libghc-mtl-doc libghc-mtl-prof libghc-network-doc libghc-network-prof libghc-network-uri-doc libghc-network-uri-prof
  libghc-objectname-doc libghc-objectname-prof libghc-old-locale-doc libghc-old-locale-prof libghc-old-time-doc libghc-old-time-prof libghc-opengl-doc libghc-opengl-prof
  libghc-openglraw-doc libghc-openglraw-prof libghc-parallel-doc libghc-parallel-prof libghc-parsec3-doc libghc-parsec3-prof libghc-primitive-doc libghc-primitive-prof
  libghc-quickcheck2-doc libghc-quickcheck2-prof libghc-random-doc libghc-random-prof libghc-regex-base-doc libghc-regex-base-prof libghc-regex-compat-doc
  libghc-regex-compat-prof libghc-regex-posix-doc libghc-regex-posix-prof libghc-scientific-doc libghc-scientific-prof libghc-split-doc libghc-split-prof
  libghc-statevar-doc libghc-statevar-prof libghc-stm-doc libghc-stm-prof libghc-syb-doc libghc-syb-prof libghc-text-doc libghc-text-prof libghc-tf-random-doc
  libghc-tf-random-prof libghc-unordered-containers-doc libghc-unordered-containers-prof libghc-vector-doc libghc-vector-prof libghc-zlib-doc libghc-zlib-prof
The following NEW packages will be installed
  alex cabal-install ghc happy haskell-platform hscolour libbsd-dev libghc-async-dev libghc-attoparsec-dev libghc-case-insensitive-dev libghc-fgl-dev libghc-gluraw-dev
  libghc-glut-dev libghc-hashable-dev libghc-haskell-src-dev libghc-html-dev libghc-http-dev libghc-hunit-dev libghc-mtl-dev libghc-network-dev libghc-network-uri-dev
  libghc-objectname-dev libghc-old-locale-dev libghc-old-time-dev libghc-opengl-dev libghc-openglraw-dev libghc-parallel-dev libghc-parsec3-dev libghc-primitive-dev
  libghc-quickcheck2-dev libghc-random-dev libghc-regex-base-dev libghc-regex-compat-dev libghc-regex-posix-dev libghc-scientific-dev libghc-split-dev libghc-statevar-dev
  libghc-stm-dev libghc-syb-dev libghc-text-dev libghc-tf-random-dev libghc-unordered-containers-dev libghc-vector-dev libghc-zlib-dev libxi-dev libxmu-dev libxmu-headers
0 to upgrade, 47 to newly install, 0 to remove and 64 not to upgrade.
Need to get 54.4 MB of archives.
After this operation, 631 MB of additional disk space will be used.
Do you want to continue? [Y/n] 


```

