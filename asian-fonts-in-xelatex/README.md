## Asian Fonts in Xelatex

I generally used xelatex for using Burmese, Khmer and Thai fonts.  
Check and learn how to use Asian fonts in latex with this latex source file: [asian-font-eg.tex](https://github.com/ye-kyaw-thu/latex-examples/blob/main/asian-fonts-in-xelatex/asian-font-eg.tex)   

I hope this example file is useful for you.  

ye@LST, NECTEC  
28 July 2022  

The followings are some commands that I used when I prepared this example file.  

## Compile the Latex Source

```
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$ xelatex ./asian-font-eg.tex 
This is XeTeX, Version 3.14159265-2.6-0.99998 (TeX Live 2017/Debian) (preloaded format=xelatex)
 restricted \write18 enabled.
entering extended mode
(./asian-font-eg.tex
LaTeX2e <2017-04-15>
Babel <3.18> and hyphenation patterns for 26 language(s) loaded.
(/usr/share/texlive/texmf-dist/tex/latex/base/article.cls
Document Class: article 2014/09/29 v1.4h Standard LaTeX document class
(/usr/share/texlive/texmf-dist/tex/latex/base/size12.clo))
(/usr/share/texlive/texmf-dist/tex/latex/fontspec/fontspec.sty
(/usr/share/texlive/texmf-dist/tex/latex/l3packages/xparse/xparse.sty
(/usr/share/texlive/texmf-dist/tex/latex/l3kernel/expl3.sty
(/usr/share/texlive/texmf-dist/tex/latex/l3kernel/expl3-code.tex)
(/usr/share/texlive/texmf-dist/tex/latex/l3kernel/l3xdvipdfmx.def)))
(/usr/share/texlive/texmf-dist/tex/latex/fontspec/fontspec-xetex.sty
(/usr/share/texlive/texmf-dist/tex/latex/base/fontenc.sty
(/usr/share/texlive/texmf-dist/tex/latex/base/tuenc.def))
(/usr/share/texlive/texmf-dist/tex/latex/fontspec/fontspec.cfg)))
(/usr/share/texlive/texmf-dist/tex/latex/base/inputenc.sty

Package inputenc Warning: inputenc package ignored with utf8 based engines.

)

Package inputenc Warning: inputenc package ignored with utf8 based engines.

(/usr/share/texlive/texmf-dist/tex/xelatex/xecjk/xeCJK.sty
(/usr/share/texlive/texmf-dist/tex/latex/l3packages/xtemplate/xtemplate.sty)
(/usr/share/texlive/texmf-dist/tex/latex/l3packages/l3keys2e/l3keys2e.sty)
(/usr/share/texlive/texmf-dist/tex/xelatex/xecjk/xunicode-addon.sty
(/usr/share/texlive/texmf-dist/tex/xelatex/xunicode/xunicode.sty
*** you should *not* be loading the inputenc package
*** XeTeX expects the source to be in UTF8 encoding
*** some features of other encodings may conflict, resulting in poor output.
(/usr/share/texmf/tex/latex/tipa/t3enc.def)
(/usr/share/texlive/texmf-dist/tex/latex/graphics/graphicx.sty
(/usr/share/texlive/texmf-dist/tex/latex/graphics/keyval.sty)
(/usr/share/texlive/texmf-dist/tex/latex/graphics/graphics.sty
(/usr/share/texlive/texmf-dist/tex/latex/graphics/trig.sty)
(/usr/share/texlive/texmf-dist/tex/latex/graphics-cfg/graphics.cfg)
(/usr/share/texlive/texmf-dist/tex/latex/graphics-def/xetex.def)))))
(/usr/share/texlive/texmf-dist/tex/xelatex/xunicode/xunicode.sty
*** Reloading Xunicode for encoding 'TU' ***
) (/usr/share/texlive/texmf-dist/tex/xelatex/xecjk/xunicode-extra.def)
(/usr/share/texlive/texmf-dist/tex/xelatex/xecjk/xeCJK.cfg))
*************************************************
* fontspec warning: "script-not-exist"
* 
* Font 'UnGungseo' does not contain script 'CJK'.
*************************************************
(./asian-font-eg.aux) (/usr/share/texmf/tex/latex/tipa/t3cmr.fd)
*** you should *not* be loading the inputenc package
*** XeTeX expects the source to be in UTF8 encoding
*** some features of other encodings may conflict, resulting in poor output.

Underfull \hbox (badness 10000) in paragraph at lines 58--59


Underfull \hbox (badness 10000) in paragraph at lines 62--63


Underfull \hbox (badness 10000) in paragraph at lines 70--73


Underfull \hbox (badness 10000) in paragraph at lines 76--79

[1] (./asian-font-eg.aux) )
(see the transcript file for additional information)
Output written on asian-font-eg.pdf (1 page).
Transcript written on asian-font-eg.log.
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$
```

## Opening the Compiled PDF File

```
evince ./asian-font-eg.pdf
```

## Installing Microsoft Core Fonts 

```
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$ sudo apt install ttf-mscorefonts-installer
[sudo] password for ye: 
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following packages were automatically installed and are no longer required:
  linux-hwe-5.4-headers-5.4.0-117 linux-hwe-5.4-headers-5.4.0-120
Use 'sudo apt autoremove' to remove them.
The following additional packages will be installed:
  cabextract libmspack0
The following NEW packages will be installed:
  cabextract libmspack0 ttf-mscorefonts-installer
0 upgraded, 3 newly installed, 0 to remove and 140 not upgraded.
Need to get 86.8 kB of archives.
After this operation, 261 kB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 http://mm.archive.ubuntu.com/ubuntu bionic-updates/main amd64 libmspack0 amd64 0.6-3ubuntu0.3 [37.5 kB]
Get:2 http://mm.archive.ubuntu.com/ubuntu bionic/universe amd64 cabextract amd64 1.6-1.1 [21.8 kB]
Get:3 http://mm.archive.ubuntu.com/ubuntu bionic/multiverse amd64 ttf-mscorefonts-installer all 3.6ubuntu2 [27.6 kB]
Fetched 86.8 kB in 1s (60.3 kB/s)                 
Preconfiguring packages ...
Selecting previously unselected package libmspack0:amd64.
(Reading database ... 452925 files and directories currently installed.)
Preparing to unpack .../libmspack0_0.6-3ubuntu0.3_amd64.deb ...
Unpacking libmspack0:amd64 (0.6-3ubuntu0.3) ...
Selecting previously unselected package cabextract.
Preparing to unpack .../cabextract_1.6-1.1_amd64.deb ...
Unpacking cabextract (1.6-1.1) ...
Selecting previously unselected package ttf-mscorefonts-installer.
Preparing to unpack .../ttf-mscorefonts-installer_3.6ubuntu2_all.deb ...
Unpacking ttf-mscorefonts-installer (3.6ubuntu2) ...
Setting up libmspack0:amd64 (0.6-3ubuntu0.3) ...
Setting up cabextract (1.6-1.1) ...
Setting up ttf-mscorefonts-installer (3.6ubuntu2) ...
Processing triggers for update-notifier-common (3.192.1.7) ...
ttf-mscorefonts-installer: processing...
ttf-mscorefonts-installer: downloading http://downloads.sourceforge.net/corefonts/andale32.exe
Get:1 http://downloads.sourceforge.net/corefonts/andale32.exe [198 kB]
Fetched 198 kB in 2s (87.1 kB/s)                                                              
ttf-mscorefonts-installer: downloading http://downloads.sourceforge.net/corefonts/arial32.exe
Get:1 http://downloads.sourceforge.net/corefonts/arial32.exe [554 kB]
Fetched 554 kB in 2s (231 kB/s)                                                              
ttf-mscorefonts-installer: downloading http://downloads.sourceforge.net/corefonts/arialb32.exe
Get:1 http://downloads.sourceforge.net/corefonts/arialb32.exe [168 kB]
Fetched 168 kB in 1s (134 kB/s)                                                              
ttf-mscorefonts-installer: downloading http://downloads.sourceforge.net/corefonts/comic32.exe
Get:1 http://downloads.sourceforge.net/corefonts/comic32.exe [246 kB]
Fetched 246 kB in 2s (162 kB/s)                                                             
ttf-mscorefonts-installer: downloading http://downloads.sourceforge.net/corefonts/courie32.exe
Get:1 http://downloads.sourceforge.net/corefonts/courie32.exe [646 kB]
Fetched 646 kB in 3s (203 kB/s)                                                               
ttf-mscorefonts-installer: downloading http://downloads.sourceforge.net/corefonts/georgi32.exe
Get:1 http://downloads.sourceforge.net/corefonts/georgi32.exe [392 kB]
Fetched 392 kB in 1s (267 kB/s)                                                               
ttf-mscorefonts-installer: downloading http://downloads.sourceforge.net/corefonts/impact32.exe
Get:1 http://downloads.sourceforge.net/corefonts/impact32.exe [173 kB]
Fetched 173 kB in 1s (126 kB/s)                                                              
ttf-mscorefonts-installer: downloading http://downloads.sourceforge.net/corefonts/times32.exe
Get:1 http://downloads.sourceforge.net/corefonts/times32.exe [662 kB]
Fetched 662 kB in 3s (244 kB/s)                                                              
ttf-mscorefonts-installer: downloading http://downloads.sourceforge.net/corefonts/trebuc32.exe
Get:1 http://downloads.sourceforge.net/corefonts/trebuc32.exe [357 kB]
Fetched 357 kB in 2s (233 kB/s)                                                               
ttf-mscorefonts-installer: downloading http://downloads.sourceforge.net/corefonts/verdan32.exe
Get:1 http://downloads.sourceforge.net/corefonts/verdan32.exe [352 kB]
Fetched 352 kB in 2s (227 kB/s)                                                               
ttf-mscorefonts-installer: downloading http://downloads.sourceforge.net/corefonts/webdin32.exe
Get:1 http://downloads.sourceforge.net/corefonts/webdin32.exe [185 kB]
Fetched 185 kB in 1s (145 kB/s)                                                              

These fonts were provided by Microsoft "in the interest of cross-
platform compatibility".  This is no longer the case, but they are
still available from third parties.

You are free to download these fonts and use them for your own use,
but you may not redistribute them in modified form, including changes
to the file name or packaging format.

Extracting cabinet: /var/lib/update-notifier/package-data-downloads/partial/andale32.exe
  extracting fontinst.inf
  extracting andale.inf
  extracting fontinst.exe
  extracting AndaleMo.TTF
  extracting ADVPACK.DLL
  extracting W95INF32.DLL
  extracting W95INF16.DLL

All done, no errors.
Extracting cabinet: /var/lib/update-notifier/package-data-downloads/partial/arial32.exe
  extracting FONTINST.EXE
  extracting fontinst.inf
  extracting Ariali.TTF
  extracting Arialbd.TTF
  extracting Arialbi.TTF
  extracting Arial.TTF

All done, no errors.
Extracting cabinet: /var/lib/update-notifier/package-data-downloads/partial/arialb32.exe
  extracting fontinst.exe
  extracting fontinst.inf
  extracting AriBlk.TTF

All done, no errors.
Extracting cabinet: /var/lib/update-notifier/package-data-downloads/partial/comic32.exe
  extracting fontinst.inf
  extracting Comicbd.TTF
  extracting Comic.TTF
  extracting fontinst.exe

All done, no errors.
Extracting cabinet: /var/lib/update-notifier/package-data-downloads/partial/courie32.exe
  extracting cour.ttf
  extracting courbd.ttf
  extracting courbi.ttf
  extracting fontinst.inf
  extracting couri.ttf
  extracting fontinst.exe

All done, no errors.
Extracting cabinet: /var/lib/update-notifier/package-data-downloads/partial/georgi32.exe
  extracting fontinst.inf
  extracting Georgiaz.TTF
  extracting Georgiab.TTF
  extracting Georgiai.TTF
  extracting Georgia.TTF
  extracting fontinst.exe

All done, no errors.
Extracting cabinet: /var/lib/update-notifier/package-data-downloads/partial/impact32.exe
  extracting fontinst.exe
  extracting Impact.TTF
  extracting fontinst.inf

All done, no errors.
Extracting cabinet: /var/lib/update-notifier/package-data-downloads/partial/times32.exe
  extracting fontinst.inf
  extracting Times.TTF
  extracting Timesbd.TTF
  extracting Timesbi.TTF
  extracting Timesi.TTF
  extracting FONTINST.EXE

All done, no errors.
Extracting cabinet: /var/lib/update-notifier/package-data-downloads/partial/trebuc32.exe
  extracting FONTINST.EXE
  extracting trebuc.ttf
  extracting Trebucbd.ttf
  extracting trebucbi.ttf
  extracting trebucit.ttf
  extracting fontinst.inf

All done, no errors.
Extracting cabinet: /var/lib/update-notifier/package-data-downloads/partial/verdan32.exe
  extracting fontinst.exe
  extracting fontinst.inf
  extracting Verdanab.TTF
  extracting Verdanai.TTF
  extracting Verdanaz.TTF
  extracting Verdana.TTF

All done, no errors.
Extracting cabinet: /var/lib/update-notifier/package-data-downloads/partial/webdin32.exe
  extracting fontinst.exe
  extracting Webdings.TTF
  extracting fontinst.inf
  extracting Licen.TXT

All done, no errors.
All fonts downloaded and installed.
Processing triggers for libc-bin (2.27-3ubuntu1.5) ...
/sbin/ldconfig.real: /usr/local/lib/libwx_gtk2u_ribbon-3.0.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libwx_gtk2u_html-3.0.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libwx_gtk2u_adv-3.0.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libwx_gtk2u_aui-3.0.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libpialign.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libwx_gtk2u_richtext-3.0.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libwx_gtk2u_xrc-3.0.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libwx_gtk2u_qa-3.0.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libwx_baseu_net-3.0.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libwx_baseu_xml-3.0.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libwx_gtk2u_core-3.0.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libwx_gtk2u_stc-3.0.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libwx_gtk2u_gl-3.0.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libwx_gtk2u_propgrid-3.0.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/liboll.so.0 is not a symbolic link

/sbin/ldconfig.real: /usr/local/lib/libwx_baseu-3.0.so.0 is not a symbolic link

Processing triggers for man-db (2.8.3-2ubuntu0.1) ...
Processing triggers for fontconfig (2.12.6-0ubuntu2) ...
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$ 
```

## Installation of Khmer OS Fonts

```
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$ sudo apt-get install fonts-khmeros-core
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following packages were automatically installed and are no longer required:
  linux-hwe-5.4-headers-5.4.0-117 linux-hwe-5.4-headers-5.4.0-120
Use 'sudo apt autoremove' to remove them.
The following NEW packages will be installed:
  fonts-khmeros-core
0 upgraded, 1 newly installed, 0 to remove and 140 not upgraded.
Need to get 91.2 kB of archives.
After this operation, 585 kB of additional disk space will be used.
Get:1 http://mm.archive.ubuntu.com/ubuntu bionic/main amd64 fonts-khmeros-core all 5.0-7ubuntu1 [91.2 kB]
Fetched 91.2 kB in 1s (80.6 kB/s)             
Selecting previously unselected package fonts-khmeros-core.
(Reading database ... 452950 files and directories currently installed.)
Preparing to unpack .../fonts-khmeros-core_5.0-7ubuntu1_all.deb ...
Unpacking fonts-khmeros-core (5.0-7ubuntu1) ...
Setting up fonts-khmeros-core (5.0-7ubuntu1) ...
Processing triggers for fontconfig (2.12.6-0ubuntu2) ...
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$
```

## Example Removing of Khmer OS Fonts

```
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$ sudo apt-get remove fonts-khmeros-core 
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following packages were automatically installed and are no longer required:
  linux-hwe-5.4-headers-5.4.0-117 linux-hwe-5.4-headers-5.4.0-120
Use 'sudo apt autoremove' to remove them.
The following packages will be REMOVED:
  fonts-khmeros-core
0 upgraded, 0 newly installed, 1 to remove and 140 not upgraded.
After this operation, 585 kB disk space will be freed.
Do you want to continue? [Y/n] Y
(Reading database ... 452955 files and directories currently installed.)
Removing fonts-khmeros-core (5.0-7ubuntu1) ...
Processing triggers for fontconfig (2.12.6-0ubuntu2) ...
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$ 
```

## Installation latex-cjk-all

```
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$ sudo apt-get install latex-cjk-all
[sudo] password for ye: 
Reading package lists... Done
Building dependency tree       
Reading state information... Done
latex-cjk-all is already the newest version (4.8.4+git20170127-2).
The following packages were automatically installed and are no longer required:
  linux-hwe-5.4-headers-5.4.0-117 linux-hwe-5.4-headers-5.4.0-120
Use 'sudo apt autoremove' to remove them.
0 upgraded, 0 newly installed, 0 to remove and 140 not upgraded.
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$
```

## Installation of Korean Fonts

```
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$ sudo apt-get install korean*
Reading package lists... Done
Building dependency tree       
Reading state information... Done
Note, selecting 'cmap-adobe-korea1' for regex 'korean*'
Note, selecting 'texlive-lang-korean' for regex 'korean*'
Note, selecting 'latex-cjk-korean' for regex 'korean*'
Note, selecting 'poppler-data' instead of 'cmap-adobe-korea1'
poppler-data is already the newest version (0.4.8-2).
poppler-data set to manually installed.
latex-cjk-korean is already the newest version (4.8.4+git20170127-2).
latex-cjk-korean set to manually installed.
texlive-lang-korean is already the newest version (2017.20180305-1).
texlive-lang-korean set to manually installed.
The following packages were automatically installed and are no longer required:
  linux-hwe-5.4-headers-5.4.0-117 linux-hwe-5.4-headers-5.4.0-120
Use 'sudo apt autoremove' to remove them.
0 upgraded, 0 newly installed, 0 to remove and 140 not upgraded.
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$ 
```

```
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$ sudo apt-get install language-pack-ko
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following packages were automatically installed and are no longer required:
  linux-hwe-5.4-headers-5.4.0-117 linux-hwe-5.4-headers-5.4.0-120
Use 'sudo apt autoremove' to remove them.
The following additional packages will be installed:
  language-pack-ko-base
The following NEW packages will be installed:
  language-pack-ko language-pack-ko-base
0 upgraded, 2 newly installed, 0 to remove and 140 not upgraded.
Need to get 914 kB of archives.
After this operation, 3,890 kB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 http://mm.archive.ubuntu.com/ubuntu bionic-updates/main amd64 language-pack-ko-base all 1:18.04+20180712 [912 kB]
Get:2 http://mm.archive.ubuntu.com/ubuntu bionic-updates/main amd64 language-pack-ko all 1:18.04+20180712 [1,900 B]
Fetched 914 kB in 3s (277 kB/s)              
Selecting previously unselected package language-pack-ko-base.
(Reading database ... 452956 files and directories currently installed.)
Preparing to unpack .../language-pack-ko-base_1%3a18.04+20180712_all.deb ...
Unpacking language-pack-ko-base (1:18.04+20180712) ...
Selecting previously unselected package language-pack-ko.
Preparing to unpack .../language-pack-ko_1%3a18.04+20180712_all.deb ...
Unpacking language-pack-ko (1:18.04+20180712) ...
Setting up language-pack-ko (1:18.04+20180712) ...
Setting up language-pack-ko-base (1:18.04+20180712) ...
Generating locales (this might take a while)...
  ko_KR.UTF-8... done
Generation complete.
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$
```

## Clear and Regenerate your Font Cache

```
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$ fc-cache -f -v
/usr/share/fonts: caching, new cache contents: 0 fonts, 10 dirs
/usr/share/fonts/X11: caching, new cache contents: 0 fonts, 4 dirs
/usr/share/fonts/X11/Type1: caching, new cache contents: 81 fonts, 0 dirs
/usr/share/fonts/X11/encodings: caching, new cache contents: 0 fonts, 1 dirs
/usr/share/fonts/X11/encodings/large: caching, new cache contents: 0 fonts, 0 dirs
/usr/share/fonts/X11/misc: caching, new cache contents: 89 fonts, 0 dirs
/usr/share/fonts/X11/util: caching, new cache contents: 0 fonts, 0 dirs
/usr/share/fonts/cMap: caching, new cache contents: 0 fonts, 0 dirs
/usr/share/fonts/cmap: caching, new cache contents: 0 fonts, 5 dirs
/usr/share/fonts/cmap/adobe-cns1: caching, new cache contents: 0 fonts, 0 dirs
/usr/share/fonts/cmap/adobe-gb1: caching, new cache contents: 0 fonts, 0 dirs
/usr/share/fonts/cmap/adobe-japan1: caching, new cache contents: 0 fonts, 0 dirs
/usr/share/fonts/cmap/adobe-japan2: caching, new cache contents: 0 fonts, 0 dirs
/usr/share/fonts/cmap/adobe-korea1: caching, new cache contents: 0 fonts, 0 dirs
/usr/share/fonts/eot: caching, new cache contents: 0 fonts, 1 dirs
/usr/share/fonts/eot/font-awesome: caching, new cache contents: 0 fonts, 0 dirs
/usr/share/fonts/fonts-go: caching, new cache contents: 10 fonts, 0 dirs
/usr/share/fonts/opentype: caching, new cache contents: 0 fonts, 17 dirs
/usr/share/fonts/opentype/cabin: caching, new cache contents: 8 fonts, 0 dirs
/usr/share/fonts/opentype/ebgaramond: caching, new cache contents: 10 fonts, 0 dirs
/usr/share/fonts/opentype/font-awesome: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/opentype/freefont: caching, new cache contents: 12 fonts, 0 dirs
/usr/share/fonts/opentype/gentiumplus: caching, new cache contents: 2 fonts, 0 dirs
/usr/share/fonts/opentype/ipaexfont-gothic: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/opentype/ipaexfont-mincho: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/opentype/ipafont-gothic: caching, new cache contents: 2 fonts, 0 dirs
/usr/share/fonts/opentype/ipafont-mincho: caching, new cache contents: 2 fonts, 0 dirs
/usr/share/fonts/opentype/linux-libertine: caching, new cache contents: 13 fonts, 0 dirs
/usr/share/fonts/opentype/lobster: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/opentype/lobstertwo: caching, new cache contents: 4 fonts, 0 dirs
/usr/share/fonts/opentype/malayalam: caching, new cache contents: 3 fonts, 0 dirs
/usr/share/fonts/opentype/mathjax: caching, new cache contents: 24 fonts, 0 dirs
/usr/share/fonts/opentype/noto: caching, new cache contents: 28 fonts, 0 dirs
/usr/share/fonts/opentype/stix: caching, new cache contents: 29 fonts, 0 dirs
/usr/share/fonts/opentype/stix-word: caching, new cache contents: 5 fonts, 0 dirs
/usr/share/fonts/svg: caching, new cache contents: 0 fonts, 1 dirs
/usr/share/fonts/svg/font-awesome: caching, new cache contents: 0 fonts, 0 dirs
/usr/share/fonts/truetype: caching, new cache contents: 2 fonts, 73 dirs
/usr/share/fonts/truetype/Gargi: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/Gubbi: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/Nakula: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/Navilu: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/Sahadeva: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/Sarai: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/abyssinica: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/adf: caching, new cache contents: 44 fonts, 0 dirs
/usr/share/fonts/truetype/arphic-bkai00mp: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/arphic-bsmi00lp: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/arphic-gbsn00lp: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/arphic-gkai00mp: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/artemisia: caching, new cache contents: 4 fonts, 0 dirs
/usr/share/fonts/truetype/asana-math: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/baekmuk: caching, new cache contents: 4 fonts, 0 dirs
/usr/share/fonts/truetype/comfortaa: caching, new cache contents: 3 fonts, 0 dirs
/usr/share/fonts/truetype/complutum: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/croscore: caching, new cache contents: 12 fonts, 0 dirs
/usr/share/fonts/truetype/crosextra: caching, new cache contents: 8 fonts, 0 dirs
/usr/share/fonts/truetype/dejavu: caching, new cache contents: 22 fonts, 0 dirs
/usr/share/fonts/truetype/didot: caching, new cache contents: 4 fonts, 0 dirs
/usr/share/fonts/truetype/droid: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/ebgaramond: caching, new cache contents: 10 fonts, 0 dirs
/usr/share/fonts/truetype/font-awesome: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/fonts-beng-extra: caching, new cache contents: 6 fonts, 0 dirs
/usr/share/fonts/truetype/fonts-deva-extra: caching, new cache contents: 3 fonts, 0 dirs
/usr/share/fonts/truetype/fonts-gujr-extra: caching, new cache contents: 5 fonts, 0 dirs
/usr/share/fonts/truetype/fonts-guru-extra: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/fonts-kalapi: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/fonts-orya-extra: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/fonts-telu-extra: caching, new cache contents: 2 fonts, 0 dirs
/usr/share/fonts/truetype/freefont: caching, new cache contents: 12 fonts, 0 dirs
/usr/share/fonts/truetype/gentium: caching, new cache contents: 4 fonts, 0 dirs
/usr/share/fonts/truetype/gentium-basic: caching, new cache contents: 8 fonts, 0 dirs
/usr/share/fonts/truetype/gentiumplus: caching, new cache contents: 2 fonts, 0 dirs
/usr/share/fonts/truetype/junicode: caching, new cache contents: 4 fonts, 0 dirs
/usr/share/fonts/truetype/kacst: caching, new cache contents: 15 fonts, 0 dirs
/usr/share/fonts/truetype/kacst-one: caching, new cache contents: 2 fonts, 0 dirs
/usr/share/fonts/truetype/lao: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/lato: caching, new cache contents: 18 fonts, 0 dirs
/usr/share/fonts/truetype/liberation: caching, new cache contents: 16 fonts, 0 dirs
/usr/share/fonts/truetype/liberation2: caching, new cache contents: 12 fonts, 0 dirs
/usr/share/fonts/truetype/lohit-assamese: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/lohit-bengali: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/lohit-devanagari: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/lohit-gujarati: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/lohit-kannada: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/lohit-malayalam: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/lohit-oriya: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/lohit-punjabi: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/lohit-tamil: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/lohit-tamil-classical: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/lohit-telugu: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/malayalam: caching, new cache contents: 11 fonts, 0 dirs
/usr/share/fonts/truetype/msttcorefonts: caching, new cache contents: 60 fonts, 0 dirs
/usr/share/fonts/truetype/neohellenic: caching, new cache contents: 4 fonts, 0 dirs
/usr/share/fonts/truetype/noto: caching, new cache contents: 156 fonts, 0 dirs
/usr/share/fonts/truetype/olga: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/open-sans: caching, new cache contents: 13 fonts, 0 dirs
/usr/share/fonts/truetype/openoffice: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/padauk: caching, new cache contents: 4 fonts, 0 dirs
/usr/share/fonts/truetype/pagul: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/roboto: caching, new cache contents: 0 fonts, 1 dirs
/usr/share/fonts/truetype/roboto/hinted: caching, new cache contents: 18 fonts, 0 dirs
/usr/share/fonts/truetype/samyak: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/samyak-fonts: caching, new cache contents: 3 fonts, 0 dirs
/usr/share/fonts/truetype/sinhala: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/solomos: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/tibetan-machine: caching, new cache contents: 1 fonts, 0 dirs
/usr/share/fonts/truetype/tlwg: caching, new cache contents: 58 fonts, 0 dirs
/usr/share/fonts/truetype/ttf-khmeros-core: caching, new cache contents: 2 fonts, 0 dirs
/usr/share/fonts/truetype/ubuntu: caching, new cache contents: 13 fonts, 0 dirs
/usr/share/fonts/truetype/unfonts-core: caching, new cache contents: 12 fonts, 0 dirs
/usr/share/fonts/truetype/unfonts-extra: caching, new cache contents: 11 fonts, 0 dirs
/usr/share/fonts/type1: caching, new cache contents: 0 fonts, 2 dirs
/usr/share/fonts/type1/gsfonts: caching, new cache contents: 35 fonts, 0 dirs
/usr/share/fonts/type1/texlive-fonts-recommended: caching, new cache contents: 12 fonts, 0 dirs
/usr/share/fonts/woff: caching, new cache contents: 0 fonts, 2 dirs
/usr/share/fonts/woff/ebgaramond: caching, new cache contents: 10 fonts, 0 dirs
/usr/share/fonts/woff/font-awesome: caching, new cache contents: 1 fonts, 0 dirs
/home/ye/tool/anaconda3/fonts: skipping, no such directory
/home/ye/.local/share/fonts: caching, new cache contents: 29 fonts, 0 dirs
/home/ye/.fonts: skipping, no such directory
/usr/share/fonts/X11: skipping, looped directory detected
/usr/share/fonts/cMap: skipping, looped directory detected
/usr/share/fonts/cmap: skipping, looped directory detected
/usr/share/fonts/eot: skipping, looped directory detected
/usr/share/fonts/fonts-go: skipping, looped directory detected
/usr/share/fonts/opentype: skipping, looped directory detected
/usr/share/fonts/svg: skipping, looped directory detected
/usr/share/fonts/truetype: skipping, looped directory detected
/usr/share/fonts/type1: skipping, looped directory detected
/usr/share/fonts/woff: skipping, looped directory detected
/usr/share/fonts/X11/Type1: skipping, looped directory detected
/usr/share/fonts/X11/encodings: skipping, looped directory detected
/usr/share/fonts/X11/misc: skipping, looped directory detected
/usr/share/fonts/X11/util: skipping, looped directory detected
/usr/share/fonts/cmap/adobe-cns1: skipping, looped directory detected
/usr/share/fonts/cmap/adobe-gb1: skipping, looped directory detected
/usr/share/fonts/cmap/adobe-japan1: skipping, looped directory detected
/usr/share/fonts/cmap/adobe-japan2: skipping, looped directory detected
/usr/share/fonts/cmap/adobe-korea1: skipping, looped directory detected
/usr/share/fonts/eot/font-awesome: skipping, looped directory detected
/usr/share/fonts/opentype/cabin: skipping, looped directory detected
/usr/share/fonts/opentype/ebgaramond: skipping, looped directory detected
/usr/share/fonts/opentype/font-awesome: skipping, looped directory detected
/usr/share/fonts/opentype/freefont: skipping, looped directory detected
/usr/share/fonts/opentype/gentiumplus: skipping, looped directory detected
/usr/share/fonts/opentype/ipaexfont-gothic: skipping, looped directory detected
/usr/share/fonts/opentype/ipaexfont-mincho: skipping, looped directory detected
/usr/share/fonts/opentype/ipafont-gothic: skipping, looped directory detected
/usr/share/fonts/opentype/ipafont-mincho: skipping, looped directory detected
/usr/share/fonts/opentype/linux-libertine: skipping, looped directory detected
/usr/share/fonts/opentype/lobster: skipping, looped directory detected
/usr/share/fonts/opentype/lobstertwo: skipping, looped directory detected
/usr/share/fonts/opentype/malayalam: skipping, looped directory detected
/usr/share/fonts/opentype/mathjax: skipping, looped directory detected
/usr/share/fonts/opentype/noto: skipping, looped directory detected
/usr/share/fonts/opentype/stix: skipping, looped directory detected
/usr/share/fonts/opentype/stix-word: skipping, looped directory detected
/usr/share/fonts/svg/font-awesome: skipping, looped directory detected
/usr/share/fonts/truetype/Gargi: skipping, looped directory detected
/usr/share/fonts/truetype/Gubbi: skipping, looped directory detected
/usr/share/fonts/truetype/Nakula: skipping, looped directory detected
/usr/share/fonts/truetype/Navilu: skipping, looped directory detected
/usr/share/fonts/truetype/Sahadeva: skipping, looped directory detected
/usr/share/fonts/truetype/Sarai: skipping, looped directory detected
/usr/share/fonts/truetype/abyssinica: skipping, looped directory detected
/usr/share/fonts/truetype/adf: skipping, looped directory detected
/usr/share/fonts/truetype/arphic-bkai00mp: skipping, looped directory detected
/usr/share/fonts/truetype/arphic-bsmi00lp: skipping, looped directory detected
/usr/share/fonts/truetype/arphic-gbsn00lp: skipping, looped directory detected
/usr/share/fonts/truetype/arphic-gkai00mp: skipping, looped directory detected
/usr/share/fonts/truetype/artemisia: skipping, looped directory detected
/usr/share/fonts/truetype/asana-math: skipping, looped directory detected
/usr/share/fonts/truetype/baekmuk: skipping, looped directory detected
/usr/share/fonts/truetype/comfortaa: skipping, looped directory detected
/usr/share/fonts/truetype/complutum: skipping, looped directory detected
/usr/share/fonts/truetype/croscore: skipping, looped directory detected
/usr/share/fonts/truetype/crosextra: skipping, looped directory detected
/usr/share/fonts/truetype/dejavu: skipping, looped directory detected
/usr/share/fonts/truetype/didot: skipping, looped directory detected
/usr/share/fonts/truetype/droid: skipping, looped directory detected
/usr/share/fonts/truetype/ebgaramond: skipping, looped directory detected
/usr/share/fonts/truetype/font-awesome: skipping, looped directory detected
/usr/share/fonts/truetype/fonts-beng-extra: skipping, looped directory detected
/usr/share/fonts/truetype/fonts-deva-extra: skipping, looped directory detected
/usr/share/fonts/truetype/fonts-gujr-extra: skipping, looped directory detected
/usr/share/fonts/truetype/fonts-guru-extra: skipping, looped directory detected
/usr/share/fonts/truetype/fonts-kalapi: skipping, looped directory detected
/usr/share/fonts/truetype/fonts-orya-extra: skipping, looped directory detected
/usr/share/fonts/truetype/fonts-telu-extra: skipping, looped directory detected
/usr/share/fonts/truetype/freefont: skipping, looped directory detected
/usr/share/fonts/truetype/gentium: skipping, looped directory detected
/usr/share/fonts/truetype/gentium-basic: skipping, looped directory detected
/usr/share/fonts/truetype/gentiumplus: skipping, looped directory detected
/usr/share/fonts/truetype/junicode: skipping, looped directory detected
/usr/share/fonts/truetype/kacst: skipping, looped directory detected
/usr/share/fonts/truetype/kacst-one: skipping, looped directory detected
/usr/share/fonts/truetype/lao: skipping, looped directory detected
/usr/share/fonts/truetype/lato: skipping, looped directory detected
/usr/share/fonts/truetype/liberation: skipping, looped directory detected
/usr/share/fonts/truetype/liberation2: skipping, looped directory detected
/usr/share/fonts/truetype/lohit-assamese: skipping, looped directory detected
/usr/share/fonts/truetype/lohit-bengali: skipping, looped directory detected
/usr/share/fonts/truetype/lohit-devanagari: skipping, looped directory detected
/usr/share/fonts/truetype/lohit-gujarati: skipping, looped directory detected
/usr/share/fonts/truetype/lohit-kannada: skipping, looped directory detected
/usr/share/fonts/truetype/lohit-malayalam: skipping, looped directory detected
/usr/share/fonts/truetype/lohit-oriya: skipping, looped directory detected
/usr/share/fonts/truetype/lohit-punjabi: skipping, looped directory detected
/usr/share/fonts/truetype/lohit-tamil: skipping, looped directory detected
/usr/share/fonts/truetype/lohit-tamil-classical: skipping, looped directory detected
/usr/share/fonts/truetype/lohit-telugu: skipping, looped directory detected
/usr/share/fonts/truetype/malayalam: skipping, looped directory detected
/usr/share/fonts/truetype/msttcorefonts: skipping, looped directory detected
/usr/share/fonts/truetype/neohellenic: skipping, looped directory detected
/usr/share/fonts/truetype/noto: skipping, looped directory detected
/usr/share/fonts/truetype/olga: skipping, looped directory detected
/usr/share/fonts/truetype/open-sans: skipping, looped directory detected
/usr/share/fonts/truetype/openoffice: skipping, looped directory detected
/usr/share/fonts/truetype/padauk: skipping, looped directory detected
/usr/share/fonts/truetype/pagul: skipping, looped directory detected
/usr/share/fonts/truetype/roboto: skipping, looped directory detected
/usr/share/fonts/truetype/samyak: skipping, looped directory detected
/usr/share/fonts/truetype/samyak-fonts: skipping, looped directory detected
/usr/share/fonts/truetype/sinhala: skipping, looped directory detected
/usr/share/fonts/truetype/solomos: skipping, looped directory detected
/usr/share/fonts/truetype/tibetan-machine: skipping, looped directory detected
/usr/share/fonts/truetype/tlwg: skipping, looped directory detected
/usr/share/fonts/truetype/ttf-khmeros-core: skipping, looped directory detected
/usr/share/fonts/truetype/ubuntu: skipping, looped directory detected
/usr/share/fonts/truetype/unfonts-core: skipping, looped directory detected
/usr/share/fonts/truetype/unfonts-extra: skipping, looped directory detected
/usr/share/fonts/type1/gsfonts: skipping, looped directory detected
/usr/share/fonts/type1/texlive-fonts-recommended: skipping, looped directory detected
/usr/share/fonts/woff/ebgaramond: skipping, looped directory detected
/usr/share/fonts/woff/font-awesome: skipping, looped directory detected
/usr/share/fonts/X11/encodings/large: skipping, looped directory detected
/usr/share/fonts/truetype/roboto/hinted: skipping, looped directory detected
/home/ye/tool/anaconda3/var/cache/fontconfig: cleaning cache directory
/home/ye/.cache/fontconfig: cleaning cache directory
/home/ye/.cache/fontconfig: invalid cache file: 0d8c3b2ac0904cb8a57a757ad11a4a08-le64.cache-7
/home/ye/.cache/fontconfig: invalid cache file: 7ef2298fde41cc6eeb7af42e48b7d293-le64.cache-7
/home/ye/.fontconfig: not cleaning non-existent cache directory
fc-cache: succeeded
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$
```

## List Installed Fonts

```
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$ fc-list :lang=my
/usr/share/fonts/truetype/padauk/PadaukBook-Regular.ttf: Padauk Book:style=Regular
/usr/share/fonts/truetype/noto/NotoSansMyanmar-Bold.ttf: Noto Sans Myanmar:style=Bold
/usr/share/fonts/truetype/padauk/Padauk-Bold.ttf: Padauk:style=Bold
/home/ye/.local/share/fonts/myanmar3.ttf: Myanmar3:style=Regular
/home/ye/.local/share/fonts/Pyidaungsu-1.8.3_Numbers.ttf: Pyidaungsu Numbers:style=Regular
/usr/share/fonts/truetype/noto/NotoSerifMyanmar-Bold.ttf: Noto Serif Myanmar:style=Bold
/home/ye/.local/share/fonts/Pyidaungsu-1.8.3_Regular.ttf: Pyidaungsu:style=Regular
/home/ye/.local/share/fonts/Mon.ttf: Mon:style=Regular,Normal
/usr/share/fonts/truetype/noto/NotoSansMyanmarUI-Regular.ttf: Noto Sans Myanmar UI:style=Regular
/usr/share/fonts/truetype/noto/NotoSansMyanmar-Regular.ttf: Noto Sans Myanmar:style=Regular
/usr/share/fonts/truetype/padauk/Padauk-Regular.ttf: Padauk:style=Regular
/usr/share/fonts/truetype/noto/NotoSansMyanmarUI-Bold.ttf: Noto Sans Myanmar UI:style=Bold
/usr/share/fonts/truetype/noto/NotoSerifMyanmar-Regular.ttf: Noto Serif Myanmar:style=Regular
/usr/share/fonts/truetype/padauk/PadaukBook-Bold.ttf: Padauk Book:style=Bold
/home/ye/.local/share/fonts/Pyidaungsu-1.8.3_Bold.ttf: Pyidaungsu:style=Bold
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$
```

## List Installed Thai Fonts

```
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$ fc-list :lang=th
/usr/share/fonts/truetype/tlwg/TlwgTypo-Bold.ttf: Tlwg Typo:style=Bold
/usr/share/fonts/truetype/noto/NotoSansThai-Regular.ttf: Noto Sans Thai:style=Regular
/usr/share/fonts/X11/misc/7x14.pcf.gz: Fixed:style=Regular
/usr/share/fonts/truetype/tlwg/TlwgTypewriter-BoldOblique.ttf: Tlwg Typewriter:style=Bold Oblique
/usr/share/fonts/truetype/noto/NotoSansThaiUI-Bold.ttf: Noto Sans Thai UI:style=Bold
/usr/share/fonts/truetype/tlwg/Garuda.ttf: Garuda:style=Regular
/usr/share/fonts/truetype/noto/NotoSansThaiUI-Regular.ttf: Noto Sans Thai UI:style=Regular
/usr/share/fonts/truetype/tlwg/TlwgTypist.ttf: Tlwg Typist:style=Regular
/usr/share/fonts/truetype/freefont/FreeSerifItalic.ttf: FreeSerif:style=Italic,Kursiv
/usr/share/fonts/truetype/tlwg/Loma-Oblique.ttf: Loma:style=Oblique
/usr/share/fonts/X11/misc/7x13.pcf.gz: Fixed:style=Regular
/usr/share/fonts/X11/misc/9x15B.pcf.gz: Fixed:style=Bold
/usr/share/fonts/truetype/tlwg/TlwgTypo-Oblique.ttf: Tlwg Typo:style=Oblique
/usr/share/fonts/truetype/freefont/FreeSerifBoldItalic.ttf: FreeSerif:style=Bold Italic,Félkövér dőlt
/usr/share/fonts/truetype/tlwg/Laksaman-Italic.ttf: Laksaman:style=Italic
/usr/share/fonts/truetype/tlwg/Kinnari-Italic.ttf: Kinnari:style=Italic
/usr/share/fonts/truetype/tlwg/TlwgMono-Bold.ttf: Tlwg Mono:style=Bold
/usr/share/fonts/truetype/tlwg/Waree.ttf: Waree:style=Regular
/usr/share/fonts/X11/misc/7x13B.pcf.gz: Fixed:style=Bold
/usr/share/fonts/truetype/tlwg/Kinnari-Oblique.ttf: Kinnari:style=Oblique
/usr/share/fonts/X11/misc/cu12.pcf.gz: ClearlyU:style=Regular
/usr/share/fonts/truetype/tlwg/Umpush-BoldOblique.ttf: Umpush:style=Bold Oblique
/usr/share/fonts/truetype/tlwg/Umpush-Oblique.ttf: Umpush:style=Oblique
/usr/share/fonts/X11/misc/9x15.pcf.gz: Fixed:style=Regular
/usr/share/fonts/truetype/tlwg/Sawasdee-Bold.ttf: Sawasdee:style=Bold
/usr/share/fonts/X11/misc/9x18B.pcf.gz: Fixed:style=Bold
/usr/share/fonts/truetype/noto/NotoSansThai-Bold.ttf: Noto Sans Thai:style=Bold
/usr/share/fonts/X11/misc/8x13B.pcf.gz: Fixed:style=Bold
/usr/share/fonts/opentype/freefont/FreeSerifBoldItalic.otf: FreeSerif:style=Bold Italic,Félkövér dőlt
/usr/share/fonts/truetype/tlwg/Norasi-BoldItalic.ttf: Norasi:style=Bold Italic
/usr/share/fonts/X11/misc/9x18.pcf.gz: Fixed:style=Regular
/usr/share/fonts/truetype/tlwg/Laksaman-Bold.ttf: Laksaman:style=Bold
/usr/share/fonts/truetype/tlwg/Purisa-Bold.ttf: Purisa:style=Bold
/usr/share/fonts/X11/misc/10x20.pcf.gz: Fixed:style=Regular
/usr/share/fonts/truetype/tlwg/Waree-Oblique.ttf: Waree:style=Oblique
/home/ye/.local/share/fonts/Mon.ttf: Mon:style=Regular,Normal
/usr/share/fonts/truetype/tlwg/Norasi-BoldOblique.ttf: Norasi:style=Bold Oblique
/usr/share/fonts/truetype/tlwg/Garuda-Bold.ttf: Garuda:style=Bold
/usr/share/fonts/truetype/tlwg/Loma.ttf: Loma:style=Regular
/usr/share/fonts/truetype/tlwg/TlwgTypist-Oblique.ttf: Tlwg Typist:style=Oblique
/home/ye/.local/share/fonts/THSarabun.ttf: TH SarabunPSK:style=Regular
/usr/share/fonts/opentype/freefont/FreeSerif.otf: FreeSerif:style=Regular
/usr/share/fonts/X11/misc/6x13.pcf.gz: Fixed:style=SemiCondensed
/usr/share/fonts/truetype/tlwg/Purisa-BoldOblique.ttf: Purisa:style=Bold Oblique
/usr/share/fonts/X11/misc/7x13O.pcf.gz: Fixed:style=Oblique
/usr/share/fonts/truetype/tlwg/TlwgTypewriter-Bold.ttf: Tlwg Typewriter:style=Bold
/usr/share/fonts/truetype/tlwg/TlwgTypo.ttf: Tlwg Typo:style=Regular
/usr/share/fonts/truetype/tlwg/Norasi-Bold.ttf: Norasi:style=Bold
/usr/share/fonts/truetype/tlwg/Sawasdee-Oblique.ttf: Sawasdee:style=Oblique
/usr/share/fonts/truetype/tlwg/Kinnari-Bold.ttf: Kinnari:style=Bold
/usr/share/fonts/truetype/tlwg/Umpush-Light.ttf: Umpush:style=Light
/usr/share/fonts/truetype/freefont/FreeSerif.ttf: FreeSerif:style=Regular
/usr/share/fonts/truetype/tlwg/Waree-BoldOblique.ttf: Waree:style=Bold Oblique
/usr/share/fonts/truetype/tlwg/Garuda-Oblique.ttf: Garuda:style=Oblique
/usr/share/fonts/X11/misc/8x13O.pcf.gz: Fixed:style=Oblique
/usr/share/fonts/truetype/tlwg/Norasi.ttf: Norasi:style=Regular
/usr/share/fonts/truetype/noto/NotoSerifThai-Bold.ttf: Noto Serif Thai:style=Bold
/usr/share/fonts/truetype/tlwg/Garuda-BoldOblique.ttf: Garuda:style=Bold Oblique
/usr/share/fonts/truetype/tlwg/Laksaman-BoldItalic.ttf: Laksaman:style=Bold Italic
/usr/share/fonts/opentype/freefont/FreeSerifBold.otf: FreeSerif:style=Bold,Fett
/usr/share/fonts/truetype/lao/Phetsarath_OT.ttf: Phetsarath OT:style=Regular,Normal
/usr/share/fonts/truetype/tlwg/Sawasdee-BoldOblique.ttf: Sawasdee:style=Bold Oblique
/usr/share/fonts/truetype/tlwg/TlwgTypist-Bold.ttf: Tlwg Typist:style=Bold
/usr/share/fonts/truetype/tlwg/Sawasdee.ttf: Sawasdee:style=Regular
/usr/share/fonts/truetype/tlwg/TlwgMono.ttf: Tlwg Mono:style=Regular
/usr/share/fonts/truetype/tlwg/Umpush-Bold.ttf: Umpush:style=Bold
/usr/share/fonts/truetype/tlwg/TlwgMono-Oblique.ttf: Tlwg Mono:style=Oblique
/usr/share/fonts/truetype/tlwg/TlwgTypewriter.ttf: Tlwg Typewriter:style=Regular
/usr/share/fonts/truetype/tlwg/Kinnari.ttf: Kinnari:style=Regular
/usr/share/fonts/truetype/tlwg/Purisa.ttf: Purisa:style=Regular
/usr/share/fonts/truetype/tlwg/Norasi-Oblique.ttf: Norasi:style=Oblique
/usr/share/fonts/truetype/tlwg/Loma-Bold.ttf: Loma:style=Bold
/usr/share/fonts/opentype/freefont/FreeSerifItalic.otf: FreeSerif:style=Italic,Kursiv
/usr/share/fonts/truetype/tlwg/Purisa-Oblique.ttf: Purisa:style=Oblique
/usr/share/fonts/truetype/tlwg/TlwgMono-BoldOblique.ttf: Tlwg Mono:style=Bold Oblique
/usr/share/fonts/truetype/tlwg/Norasi-Italic.ttf: Norasi:style=Italic
/usr/share/fonts/X11/misc/8x13.pcf.gz: Fixed:style=Regular
/usr/share/fonts/truetype/tlwg/Laksaman.ttf: Laksaman:style=Regular
/usr/share/fonts/truetype/tlwg/Kinnari-BoldOblique.ttf: Kinnari:style=Bold Oblique
/usr/share/fonts/truetype/tlwg/Kinnari-BoldItalic.ttf: Kinnari:style=Bold Italic
/usr/share/fonts/truetype/tlwg/Loma-BoldOblique.ttf: Loma:style=Bold Oblique
/usr/share/fonts/truetype/tlwg/TlwgTypo-BoldOblique.ttf: Tlwg Typo:style=Bold Oblique
/usr/share/fonts/X11/misc/7x14B.pcf.gz: Fixed:style=Bold
/usr/share/fonts/truetype/noto/NotoSerifThai-Regular.ttf: Noto Serif Thai:style=Regular
/usr/share/fonts/truetype/tlwg/TlwgTypewriter-Oblique.ttf: Tlwg Typewriter:style=Oblique
/usr/share/fonts/truetype/freefont/FreeSerifBold.ttf: FreeSerif:style=Bold,Fett
/usr/share/fonts/truetype/tlwg/TlwgTypist-BoldOblique.ttf: Tlwg Typist:style=Bold Oblique
/usr/share/fonts/truetype/tlwg/Waree-Bold.ttf: Waree:style=Bold
/usr/share/fonts/truetype/tlwg/Umpush-LightOblique.ttf: Umpush:style=Light Oblique
/usr/share/fonts/truetype/tlwg/Umpush.ttf: Umpush:style=Regular
(base) ye@ykt-pro:~/cadt/ACET/ref-latex/final-cameara-ready-KWS-NLP2015/asian-fonts-eg$
```

## References

- http://www.khmerfonts.info/
- http://khmertype.blogspot.com/
- https://medium.com/source-words/how-to-manually-install-update-and-uninstall-fonts-on-linux-a8d09a3853b0
- https://github.com/larmarange/demopaedia/blob/master/fonts/THSarabun.ttf





