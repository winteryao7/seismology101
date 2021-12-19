此节简单介绍几种常见的数据转换工具，当然上一节提到的obspy可以轻松实现转化，
但介于不同的数据采集方式，了解如何转化可以省去很多时间

evt2sac
-------

由NEIC常用的CD-ROMS转成可以直接使用的SAC格式。源代码以及安装方法可以参见_`IRIS SeisCod <https://seiscode.iris.washington.edu/projects/evt2sac>`_。
由于该格式逐渐被取代，所以源代码也没有持续的更新，IRIS已经不再维护。CD-ROMS存储的数据格式在国内还在使用，掌握简单的使用方法依然有用。

rt2ms
-----
RT130是REFTECK数据采集系统(Data Acquisition System)常见的一种数据格式。如果采用REFTECK的DAS，那么使用配套的数据处理软件会事半功倍。obspy也可以读取该类型
的数据文件，但PASSCAL提供更加便捷的rt2ms，可以直接将RT130直接转换成daily mseed格式。其安装和使用可以参考_`PASSCAL PASSOFT <https://www.passcal.nmt.edu/content/software-resources>`_。

