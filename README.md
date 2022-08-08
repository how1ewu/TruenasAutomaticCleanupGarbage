## 脚本


```shell
#!/bin/sh  

find /mnt/[MountPoint]/.recycle/* -atime +[Age] -exec rm -rf '{}' \;
find /mnt/[MountPoint]/.recycle/ -depth -type d -empty -exec rmdir {} \;
```
* 填入以下内容，[MountPoint] 替换成你挂载点的名字，[Age] 替换成天数
