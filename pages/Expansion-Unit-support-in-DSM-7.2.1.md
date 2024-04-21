https://www.reddit.com/r/synology/comments/186s6h8/comment/kbaue3c/

### Geminilake: DS1520+, DS920+ and DS720+

| File              | RX418 | DX517 | RX415 | DX513 | DX213 | Comment    |
|-------------------|-------|-------|-------|-------|-------|------------|
| model.dtb         | no    | yes   | no    | no    | no    | see Note 1 |
| synoinfo.conf     | yes   | yes   | no    | no    | no    | see Note 1 |
| scemd             | yes   | yes   | no    | no    | no    | OK see Note 2 |
| scemd.xml         | yes   | yes   | yes   | yes   | yes   | OK         |
| libhwcontrol.so.1 | yes   | yes   | yes   | yes   | yes   | OK         |
| diskaction.xml    | no    | no    | no    | yes   | yes   | OK see Note 3 |
| drive db file     | yes   | yes   | yes   | yes   | yes   | OK         |

**Notes:**
1. Use [Synology enable eunit](https://github.com/007revad/Synology_enable_eunit)
2. Works without editing scemd.
3. All NAS models have the same diskaction.xml
4. All Synology NAS models have the required drive database files.

<br>

**File locations:**

```
/etc.defaults/model.dtb
/etc.defaults/synoinfo.conf
/usr/syno/bin/scemd
/usr/syno/etc.defaults/scemd.xml
/usr/lib/libhwcontrol.so.1
/var.defaults/lib/diskaction/diskaction.xml
```

<br>
