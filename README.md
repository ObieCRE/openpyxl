This a fork of the openpyxl library. The main place this code lives is https://foss.heptapod.net/openpyxl/openpyxl

The main functionality that this fork adds is the ability to optionally ignore files with the word "STATIC" in them.


For example when loading a workbook you can use `ignore_static_files`


```py
load_workbook(self.filename, data_only=True, ignore_static_files=True)
```

This functionality was used to enable more efficient loading of large files [in a pycel fork](https://github.com/ObieCRE/pycel) we made
