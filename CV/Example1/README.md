# CV Example 1

I referred following repository:  

[https://github.com/muratcankaracabey/latex_cv](https://github.com/muratcankaracabey/latex_cv)  

The example compilation was done with my CV information.  

## Notes Based on My Compilation Errors

### Error If You Don't Have Awesome Font

```
/usr/share/texlive/texmf-dist/web2c/mktexnam: Need to update /usr/share/texlive/texmf-dist/fonts/map/fontname/special.map?
mktextfm: Running mf-nowin -progname=mf \mode:=ljfour; mag:=1; nonstopmode; input FontAwesome
This is METAFONT, Version 2.7182818 (TeX Live 2017/Debian) (preloaded base=mf)


kpathsea: Running mktexmf FontAwesome
! I can't find file `FontAwesome'.
<*> ...our; mag:=1; nonstopmode; input FontAwesome
                                                  
Please type another input file name
! Emergency stop.
<*> ...our; mag:=1; nonstopmode; input FontAwesome
                                                  
Transcript written on mfput.log.
grep: FontAwesome.log: No such file or directory
mktextfm: `mf-nowin -progname=mf \mode:=ljfour; mag:=1; nonstopmode; input FontAwesome' failed to make FontAwesome.tfm.
kpathsea: Appending font creation commands to missfont.log.


!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
!
! fontspec error: "font-not-found"
! 
! The font "FontAwesome" cannot be found.
! 
! See the fontspec documentation for further information.
! 
! For immediate help type H <return>.
!...............................................  
                                                  
l.45 \newfontfamily{\FA}{FontAwesome}
                                     
? x
No pages of output.
Transcript written on example_cover_letter.log.
(base) ye@ykt-pro:/media/ye/project2/ye-gpu/ye-cv$
```

## Solution for Above Error: Awesome Font Installation

```
(base) ye@ykt-pro:/media/ye/project2/ye-gpu/ye-cv$ sudo apt-get install -y fonts-font-awesome
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following packages were automatically installed and are no longer required:
  linux-hwe-5.4-headers-5.4.0-117 linux-hwe-5.4-headers-5.4.0-120
Use 'sudo apt autoremove' to remove them.
The following NEW packages will be installed:
  fonts-font-awesome
0 upgraded, 1 newly installed, 0 to remove and 142 not upgraded.
Need to get 0 B/513 kB of archives.
After this operation, 1,394 kB of additional disk space will be used.
Selecting previously unselected package fonts-font-awesome.
(Reading database ... 452837 files and directories currently installed.)
Preparing to unpack .../fonts-font-awesome_4.7.0~dfsg-3_all.deb ...
Unpacking fonts-font-awesome (4.7.0~dfsg-3) ...
Setting up fonts-font-awesome (4.7.0~dfsg-3) ...
Processing triggers for fontconfig (2.12.6-0ubuntu2) ...
(base) ye@ykt-pro:/media/ye/project2/ye-gpu/ye-cv$
```

## Confirmation

```
(base) ye@ykt-pro:/media/ye/project2/ye-gpu/ye-cv$ fc-cache -f -v
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
/home/ye/.local/share/fonts: caching, new cache contents: 30 fonts, 0 dirs
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
/home/ye/.cache/fontconfig: invalid cache file: 3830d5c3ddfd5cd38a049b759396e72e-le64.cache-7
/home/ye/.cache/fontconfig: invalid cache file: cba07694886bf8bbc441deea9dc5842f-le64.cache-7
/home/ye/.cache/fontconfig: invalid cache file: 573ec803664ed168555e0e8b6d0f0c7f-le64.cache-7
/home/ye/.fontconfig: not cleaning non-existent cache directory
fc-cache: succeeded
(base) ye@ykt-pro:/media/ye/project2/ye-gpu/ye-cv$ fc-list | grep "awesome"
/usr/share/fonts/opentype/font-awesome/FontAwesome.otf: FontAwesome:style=Regular
/usr/share/fonts/woff/font-awesome/fontawesome-webfont.woff: FontAwesome:style=Regular
/usr/share/fonts/truetype/font-awesome/fontawesome-webfont.ttf: FontAwesome:style=Regular
(base) ye@ykt-pro:/media/ye/project2/ye-gpu/ye-cv$ 
```

## Profile Picture Need to Make Resize

```
(base) ye@ykt-pro:/media/ye/project2/ye-gpu/ye-cv$ convert ./y.png -resize 403x393 ./y-resize.png

(base) ye@ykt-pro:/media/ye/project2/ye-gpu/ye-cv/images$ file ./y.png 
./y.png: PNG image data, 924 x 1200, 8-bit/color RGB, non-interlaced
(base) ye@ykt-pro:/media/ye/project2/ye-gpu/ye-cv/images$ file ./profilepicture.png 
./profilepicture.png: PNG image data, 303 x 393, 8-bit/color RGB, non-interlaced
(base) ye@ykt-pro:/media/ye/project2/ye-gpu/ye-cv/images$
```

မဟုတ်ရင် github, linkedIn icon ကို မပြပေးနိုင်တဲ့ error ရှိတယ်။  

