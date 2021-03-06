``-:`` 选项
===========

GMT在读入数据时，会认为第一列是X值，第二列是Y值。对于地理数据而言，即第一列是经度、第二列是纬度。

若要读入的数据中第一列是纬度、第二列是经度，则需要先交换第一列和第二列再读入，可以使用 ``-:`` 选项实现前两列数据的交换。

默认情况下，该选项同时对输入输出生效：

- ``-:i`` 表明该选项仅交换输入数据的前两列，等效于 ``-i1,0``
- ``-:o`` 表明该选项仅交换输出数据的前两列，等效于 ``-o1,0``

说明：

#. 该选项仅用于交换输入/输出的前两列数据， ``-R`` 选项中始终是经度在前，网格文件中经度始终是第一维度
