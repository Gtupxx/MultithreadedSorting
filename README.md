# 睡觉排序
- 😴 一种基于多线程的排序算法，时间复杂度为O(N)，只是为了好玩
- ⏱️ 算法中只遍历了一次数据！时间复杂度O(N)！
- 🧵 有多少个元素就创建多少个线程！
- 💾 空间复杂度也是O(N)！
- ⚠️ 不建议在实际生产时使用此函数😙

# 使用例：
- 假设*data*是一个**vector<int>**类型的数组，存放着要排序的数据；
- *accu*是一个**int**类型的变量，表示线程“睡觉”时放大的倍率；
   - 这个参数可以根据所需的精度来设定，accu越大，精度越高，出错的可能性越小；
   - 例如某个要排序的元素x，它所对应的线程要“睡觉”的时间$t=accu\times x$(毫秒)。
- SleepSort(data,accu); //data是引用传参，排序后的数据仍然存放在data里。
