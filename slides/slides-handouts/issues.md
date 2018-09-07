

#issue 1

```
$ make
pandoc sample.md -t beamer --slide-level 2 -o sample.md.slides.pdf
! Undefined control sequence.
<recently read> \tightlist 
                           
l.183 \end{frame}

pandoc: Error producing PDF
make: *** [sample.md.slides.pdf] Error 43
```


SOL:

```
had to add

\providecommand{\tightlist}{%
  \setlength{\itemsep}{0pt}\setlength{\parskip}{0pt}}
```



OTHERSOL:

https://tex.stackexchange.com/questions/257418/error-tightlist-converting-md-file-into-pdf-using-pandoc




