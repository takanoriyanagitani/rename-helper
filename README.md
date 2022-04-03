# rename-helper

```

+--------------+
| Item Service |
+--------------+
    |
    | Item Info
    |   - Name
    |   - Store dependent info
    |       - encoding
    |       - disk usage
    |       - namespace
    |       - inode number
    |       - number of hard links
    |       - shared
    |       - read only
    |       - archived
    |       - modified
    |       - uploaded
    |       - ....
    v
+---------------------------+
| Item Content Info Service |
+---------------------------+
    |
    | Item Content Info
    |   - Number of pages
    |   - Width
    |   - Length
    |   - Location
    |   - Author
    |   - Number of sheets
    |   - SHA256
    |   - ...
    v
+--------------+
| Name Service |
+--------------+
    |
    | Rename Info
    |   - ./0001.jpg -> ./2022/04/03/0001.jpg
    |   - ./0001.png -> ./MilkeyWay/SolarSystem/Earth/.../0001.png
    |   - ./0001.jp2 -> ./resolution/fullhd/0001.jp2
    |   - ./0001.pdf -> ./2001/04/03/0001.pdf
    |   - ./0001.xls -> ./1999/04/03/0001.xls
    |   - ./0001.dat -> ./size/huge/0001.dat
    |   - ./0001.cnf -> ./user/root/0001.cnf
    |   - ./0001.lnk -> ./dup/cafef00ddeadbeafface864299792458/0001.lnk
    |   - ./zeros    -> ./sparse/2022/04/03/zeros
    |   - ./dev/sdc  -> ./type/device/dev/sdc
    |   - ...
    v
+---------------------+
| Rename Plan Service |
+---------------------+
    |
    | Rename Command
    |   - {dry:yes, src:./0001.jpg, dst:./2022/04/03/0001.jpg}
    |   - {dry:no,  ...}
    |   - ...
    v
+----------------+
| Rename Service |
+----------------+

```
