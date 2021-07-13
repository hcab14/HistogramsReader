# HistogramsReader
Saves historgrams from PM to .csv file

* Updated to "HistogramsReader2.zip"
* Moved all files into one common directory (no references to `"../*"`)
* Compiles and runs also `Ubuntu 20.04.2 LTS`; all changes for linux are within
```c++
#ifdef Q_CC_GNU
...
#endif
```

## Compilation on linux

1) install g++-9 and qt5
```
sudo apt-get install g++-9 qt5-default
```
2) build like this:
```
qmake && make -j4
```
3) start as
```
./HistogramsReader
```
and then enter the correct IPbus endpoint IP address, or edit accordingly `HistogramsReader.ini`:
```
[General]
IPaddress=127.0.0.1
```
