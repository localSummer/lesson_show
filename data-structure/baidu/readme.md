[source](https://juejin.im/book/5a8f9ddcf265da4e9f6fb959/section/5a8f9fcb6fb9a063417b3f9e#heading-10)

数据结构决定了数据存储的空间和时间效率问题， 数据的写入和提取速度也决定了应该选择怎样的数据结构
- 读得多的数据结构， 应该想办法提高数据的读取效率， 比如IP数据库， 只需要写一次， 余下都是读取
- 读bpgng都多的数据结构， 两者的平衡， LRU Cache算法


枚举和递归是最最简单的算法， 也是复杂算法的基础， 

递归由两部分组成：
1. 递归主体， 要循环解决问题的代码
2. 递归的跳出条件， 不能一直递归， 要完成一定条件后跳出。

实现JS对象的深拷贝

通过一趟排序将要排序的数据分成独立的两部分，小 pivot 大， 递归进行

A[0].....A[N-1], 选取一个数据作为关键数据，将所有比它小的数都放到它前面， 比它大的数放到后面，此为一趟，

<!-- 不是一种稳定的排序算法， 多个相同的值的相对位置也许会在算法结束时发生变动  -->

是冒泡排序的改进版， 是最快的排序方法
缺点， 不稳定

流程：
1. 随机选择数组中的一个数A, 以这个数为基准
2. 其他数字跟这个数进行比较， 比这个数小的放在其左边， 大的放在其右边
3. 经过一次循环后， A 左边为小于A的， 右边为大于A的
4. 将左边和右边的数再递归上面的地程