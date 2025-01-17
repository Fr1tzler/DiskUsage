# DiskUsage



## Требования для запуска 

Чтобы запустить утилиту необходим python версии 3.7 и выше



## Параметры запуска

**base_path** - обязательный путь

--ext нужен для вывода в конце программы размера файлов по расширениям

-s, --sort отвечает за сортировку

* name - лексикографическая
* size - размер
* fls_count - по количеству файлов

-d, --depth отвечает за глубину обхода файлов (по умолчанию 2)

 --reverse отвечает за порядок сортировки (по умолчанию True)

--noprogress отвечает за отключение прогресс бара (по умолчанию False)



## Пример работы программы

```markdown
du.py C:\Go --ext 

←[KGetting files info... |##############################  | 94/100
C:\Go\pkg (427 files) 265.2 MB
C:\Go\pkg\tool (20 files) 122.1 MB
C:\Go\pkg\windows_amd64_race (202 files) 77.3 MB
C:\Go\src (6368 files) 67.3 MB
C:\Go\pkg\windows_amd64 (202 files) 65.8 MB
C:\Go\src\cmd (2330 files) 29.2 MB
C:\Go\bin (2 files) 17.0 MB
C:\Go\api (19 files) 6.9 MB
C:\Go\test (2247 files) 5.5 MB
C:\Go\src\runtime (865 files) 4.8 MB
C:\Go\src\syscall (305 files) 4.4 MB
C:\Go\test\fixedbugs (1720 files) 3.9 MB
C:\Go\doc (147 files) 3.8 MB
C:\Go\src\crypto (358 files) 3.8 MB
C:\Go\src\vendor (171 files) 3.7 MB
C:\Go\misc (346 files) 3.2 MB
C:\Go\src\net (333 files) 2.8 MB
C:\Go\src\time (35 files) 2.7 MB
C:\Go\misc\trace (3 files) 2.6 MB
C:\Go\doc\gopher (30 files) 2.4 MB
C:\Go\src\internal (252 files) 2.3 MB
C:\Go\src\go (352 files) 1.8 MB
C:\Go\src\image (167 files) 1.3 MB
C:\Go\src\debug (105 files) 1.2 MB
C:\Go\src\math (216 files) 1.2 MB
C:\Go\src\encoding (85 files) 1.2 MB
C:\Go\src\compress (100 files) 1010.1 KB
C:\Go\lib (3 files) 765.5 KB
C:\Go\lib\time (3 files) 765.5 KB
C:\Go\src\regexp (29 files) 748.1 KB
C:\Go\src\testdata (1 files) 553.9 KB
C:\Go\src\os (147 files) 540.2 KB
C:\Go\misc\cgo (311 files) 508.3 KB
C:\Go\src\archive (92 files) 471.1 KB
C:\Go\src\html (41 files) 436.0 KB
C:\Go\src\reflect (20 files) 383.5 KB
C:\Go\src\text (27 files) 330.1 KB
C:\Go\src\database (13 files) 304.1 KB
C:\Go\src\unicode (16 files) 273.0 KB
C:\Go\src\hash (30 files) 254.9 KB
C:\Go\src\fmt (13 files) 206.0 KB
C:\Go\src\strconv (27 files) 205.4 KB
C:\Go\test\bench (23 files) 169.4 KB
C:\Go\src\testing (26 files) 166.0 KB
C:\Go\test\codegen (38 files) 156.5 KB
C:\Go\src\sync (31 files) 150.3 KB
C:\Go\src\strings (14 files) 143.3 KB
C:\Go\src\mime (29 files) 142.2 KB
C:\Go\src\bytes (10 files) 140.4 KB
C:\Go\src\path (21 files) 119.9 KB
C:\Go\src\index (6 files) 110.9 KB
C:\Go\src\bufio (6 files) 96.9 KB
C:\Go\test\ken (42 files) 92.8 KB
C:\Go\src\io (14 files) 78.5 KB
C:\Go\doc\articles (24 files) 65.7 KB
C:\Go\src\sort (17 files) 63.4 KB
C:\Go\test\chan (19 files) 60.1 KB
C:\Go\doc\codewalk (11 files) 56.0 KB
C:\Go\src\flag (5 files) 53.3 KB
C:\Go\src\context (6 files) 44.4 KB
C:\Go\doc\progs (36 files) 39.3 KB
C:\Go\src\log (8 files) 36.0 KB
C:\Go\src\container (10 files) 35.0 KB
C:\Go\misc\ios (4 files) 27.4 KB
C:\Go\test\interface (29 files) 24.6 KB
C:\Go\src\expvar (2 files) 19.6 KB
C:\Go\misc\wasm (3 files) 18.4 KB
C:\Go\src\errors (5 files) 12.1 KB
C:\Go\src\builtin (1 files) 11.0 KB
C:\Go\misc\android (2 files) 10.7 KB
C:\Go\doc\play (8 files) 10.2 KB
C:\Go\misc\chrome (8 files) 9.6 KB
C:\Go\test\stress (3 files) 9.5 KB
C:\Go\src\unsafe (1 files) 9.0 KB
C:\Go\src\plugin (4 files) 6.8 KB
C:\Go\test\closure3.dir (1 files) 6.8 KB
C:\Go\test\syntax (20 files) 6.4 KB
C:\Go\misc\reboot (3 files) 6.0 KB
C:\Go\pkg\include (3 files) 4.9 KB
C:\Go\misc\linkcheck (1 files) 4.0 KB
C:\Go\misc\swig (8 files) 3.8 KB
C:\Go\test\import2.dir (2 files) 3.1 KB
C:\Go\test\dwarf (23 files) 3.0 KB
C:\Go\test\intrinsic.dir (1 files) 2.4 KB
C:\Go\test\method4.dir (2 files) 2.3 KB
C:\Go\test\uintptrescapes.dir (2 files) 2.1 KB
C:\Go\misc\arm (1 files) 1.7 KB
C:\Go\test\alias3.dir (3 files) 1.5 KB
C:\Go\test\runtime (2 files) 961.0 Bytes
C:\Go\test\import4.dir (2 files) 923.0 Bytes
C:\Go\test\ddd2.dir (2 files) 899.0 Bytes
C:\Go\test\retjmp.dir (2 files) 847.0 Bytes
C:\Go\test\linkname.dir (3 files) 726.0 Bytes
C:\Go\test\oldescape_linkname.dir (3 files) 707.0 Bytes


Total file size by extensions:

txt : 9.5 MB
exe : 261.1 MB
html : 6.3 MB
png : 2.3 MB
css : 6.1 KB
go : 117.2 MB
mod : 2.0 KB
good : 548.0 Bytes
js : 291.1 KB
xml : 61.5 KB
jpg : 3.2 MB
gif : 100.7 KB
svg : 34.8 KB
bash : 32.5 KB
zip : 1.5 MB
f90 : 788.0 Bytes
c : 364.9 KB
h : 37.2 KB
out : 284.0 KB
s : 8.8 MB
json : 539.1 KB
sh : 99.5 KB
cc : 2.1 KB
swigcxx : 748.0 Bytes
swig : 1.1 KB
md : 85.8 KB
a : 286.3 MB
bat : 7.9 KB
rc : 4.4 KB
sum : 9.5 KB
dist : 553.0 Bytes
vendor : 2.4 KB
tar : 275.2 KB
base64 : 440.4 KB
notzip : 3.7 KB
rules : 1.6 MB
nexts : 43.7 KB
src : 385.3 KB
cov : 268.0 Bytes
golden : 407.2 KB
glock : 4.8 KB
godeps : 8.8 KB
glide : 3.4 KB
vmanifest : 2.3 KB
tsv : 19.1 KB
vconf : 13.8 KB
vyml : 1.3 KB
vjson : 115.1 KB
dep : 7.1 KB
csv : 669.8 KB
input : 163.3 KB
test : 20.5 KB
m : 2.1 KB
syso : 895.8 KB
gitignore : 188.0 Bytes
cfg : 42.0 Bytes
bz2 : 1.4 MB
bin : 262.3 KB
expect : 13.7 KB
in : 280.0 KB
gz : 358.3 KB
pem : 1.6 KB
crt : 7.6 KB
elf : 115.7 KB
elf4 : 18.5 KB
macho : 9.8 KB
obj : 142.9 KB
gox : 76.3 KB
x : 4.7 KB
raw : 24.8 KB
norm : 3.8 KB
awk : 900.0 Bytes
tmpl : 932.0 Bytes
sng : 510.5 KB
original : 5.4 KB
jpeg : 355.0 KB
types : 478.0 Bytes
plan9 : 514.0 Bytes
cgi : 4.2 KB
conf : 1.2 KB
pl : 61.2 KB
dat : 34.3 KB
py : 30.0 KB
S : 29.8 KB

```

