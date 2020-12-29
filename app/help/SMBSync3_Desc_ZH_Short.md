## 功能

SMBSync3是安卓设备的内部存储，MicroSD，USB闪存和PC/NAS通过无线局域网使用SMBv1，SMBv2或SMBv3协议。它是一个同步文件的工具。

<u>**同步是从源头到目的地的单向**</u>，可以进行镜像、移动、复制或存档。可以结合本地存储(<u>**1**</u>)、SMB和ZIP)。 

定期同步可以由SMBSync3的调度功能或外部应用程序（Tasker，AutoMagic等）启动。

- 镜像

  将源目录和文件进行三角复制（<u>***2**</u>）到目的地，复制完成后，删除源端不存在的文件和目录。

- 移动

  将源目录和文件delta-copy(<u>***2**</u>)到目的端，复制完成后删除源端文件(但源端和目的端同名、文件大小、修改日期相同的文件，不复制，复制完成后删除源目录和文件。侧的文件)。

- 拷贝

  Delta-copies(<u>***2**</u>)将源目录中的文件复制到目标目录。

- 归档

  源目录中包含的照片和视频，日期和时间为档案执行日期后7天 去目的地之前或30天之前等。但不能用ZIP作为目的地）。

<u>***1**</u> 本地存储可以是内部存储、MicroSD或USB闪存。

<u>***2**</u> 差别文件是以下三种情况之一。 

1. 文件不存在  
2. 不同的文件大小  
3. 与上次更新3秒时不同

如果应用程序不允许更改文件的最后更新时间，则在管理文件中记录文件的最后更新时间，并以此来判断差异文件。因此，如果复制SMBSync3以外的文件或没有管理文件，则会复制该文件。

## FAQs

[请参考PDF文件](https://drive.google.com/file/d/1v4-EIWuucUErSg9uYZtycsGGn9o-T_2t/view?usp=sharing)

## 文件

[请参考PDF文件](https://drive.google.com/file/d/1gIsulxyGBY-Fl0Ki7BJ50gPFWx0iQ9Tm/view?usp=sharing)

## 图书馆

- [jcifs-ng ClientLibrary](https://github.com/AgNO3/jcifs-ng)
- [jcifs-1.3.17](https://jcifs.samba.org/)
- [Zip4J 2.2.3](http://www.lingala.net/zip4j.html)
- [juniversalchardet-1.0.3](https://code.google.com/archive/p/juniversalchardet/)
- [Metadata-extractor](https://github.com/drewnoakes/metadata-extractor)