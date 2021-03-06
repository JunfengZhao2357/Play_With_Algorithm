## Problem1:
- 有一个字符串数组。将数组中的每一个字符串按照字母序排序：之后再将整个字符串数组按照字典序排序。那么时间复杂度为？
- 假设最长的字符串长度为s；数组中有n个字符串
- 对每个字符串排序：O(slogs)
- 将数组中的每一个字符串按照字母序排序：O(n*slogs)
- 将整个字符串数组按照字母序排序：O(s*nlogn)   其实在排序算法中O(nlogn)指的是比较的次数，对于int来说，那字符串会有s个字母，所以乘上s
- 时间复杂度：O(n*slogs)+O(s*nlogn)
---
## Problem2:
- 如果想在1s之内解决问题：
- O(n^2)的算法可以处理大约10^4级别的数据
- O(n)的算法可以处理大约10^8级别的数据
- O(nlogn)的算法可以处理大约10^7级别的数据
- 使用并行编程就可以减小程序运行时间
---
## Problem3:
- 递归调用是有空间复杂度的：通常递归调用了n次，在程序运行中就会保留n个状态，空间复杂度就是O(n)
- 递归的时间复杂度：如果递归函数中，只进行一次递归调用，递归深度为depth；在每个递归函数中，时间复杂度为T；则总体的时间复杂度为O(T*depth)
