地震图
======

:本节贡献者: |姚家园|\（作者）、
             |田冬冬|\（审稿）
:最近更新日期: 2021-05-31
:预计阅读时间: 2 分钟

----

地震图（seismogram）是指地震仪记录到的带有计时信息的地面质点运动（位移、速度、加速度、转动等），
也称为地震波形（seismic waveform），其本质是时间序列。一般有三个正交分量，
如南北、东西和垂直分量。

地震图 :math:`U(t)` 由三部分的卷积组成，即震源项 :math:`S(t)`\ 、
结构项 :math:`G(t)`\ 、仪器项 :math:`I(t)`\ ：

.. math::

   U(t) = S(t)*G(t)*I(t)

因此，地震图包含了震源、结构以及仪器的信息。地震学科研工作者正是通过解读地震图，
得到相关信息的。一般而言，仪器项（即仪器响应）已知，所以地震图通常用于反演震源和
结构信息。其中，结构项一般称为格林函数，只与地球内部结构有关。

地震图与元数据（metadata）共同构成了完备的地震学观测数据。
元数据包含与地震图相关的重要信息，如台站位置、仪器响应等。
