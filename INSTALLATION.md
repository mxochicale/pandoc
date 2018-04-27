Installation
---


# Ubuntu (Waiting for testing in a new machine!)
Required tools for producing the pdf

You'll need [pandoc](http://pandoc.org) (a universal document converter) and a
full [TeX distribution](https://www.tug.org/texlive/).

For pandoc, you'll also need the
[pandoc-crossref](https://github.com/lierdakil/pandoc-crossref) filter that you can
easily install with:

```
$ cabal update
$ cabal install pandoc-crossref
```

[REF](https://github.com/ReScience/ReScience-submission/tree/master/article)


Requirements to use ReScience-submission Template




# On Ubuntu 14.04 x64

* [ ] test the following installation method in a new machine
	(added:27april2018.15h28m, sorted:???.???)



## Quick Cabal Method

Following  https://github.com/jgm/pandoc/blob/master/INSTALL.md#quick-cabal-method
```
$ sudo apt-get install haskell-platform
$ cabal update
$ cabal install pandoc-crossref
```
** it takes about  an hour to do the installation

add in .bashrc the following line
```
export PATH=$HOME/.cabal/bin:$PATH
```



##  Failed Installation
```
sudo dpkg -i pandoc-1.19.2.1-1-amd64.deb
```

but only has pandoc and
pandoc           pandoc-citeproc  
Therefore I unstillad it with
```
sudo dpkg --remove pandoc
```
