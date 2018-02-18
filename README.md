# vector
编程中的容器
Vector是在java中可以实现自动增长的对象数组，vector在c++标准模板库中的部分内容，它是一个多功能的，能够操作多种数据结构和算法的模板类和函数库
(1) 矢量：具有方向性的量。
(2) 编程语言方面：vector是C++标准模板库中的部分内容，中文偶尔译作“容器”，但并不准确。它是一个多功能的，能够操作多种数据结构和算法的模板类和函数库。vector之所以被认为是一个容器，是因为它能够像容器一样存放各种类型的对象，简单地说，vector是一个能够存放任意类型的动态数组，能够增加和压缩数据。[1]  [2] 
简单的使用方法如下：
1
2
3
vector<int>test;//建立一个vector
test.push_back(1);
test.push_back(2);//把1和2压入vector这样test[0]就是1,test[1]就是2
我们可以用一个迭代器：
vector<int>::iterator iter=test.begin();//定义一个可以迭代int型vector的迭代器iter，它指向test的首位
for(;iter!=test.end();iter++) cout<<(*iter);//iter++指的是向后迭代一位，直到iter到超出末端迭代器为止，输出迭代器指向的值
我们也可以使用at访问：
1
2
3
4
vector<int>test;//建立一个vector
test.push_back(1);
test.push_back(2);//把1和2压入vector这样test[0]就是1,test[1]就是2
int i =test.at(1);//i为2
在JAVA中
Java.util.Vector提供了向量（Vector）类以实现类似动态数组的功能。在Java语言中是没有指针概念的，但如果能正确灵活地使用指针又确实可以大大提高程序的质量，比如在C、C++中所谓“动态数组”一般都由指针来实现。为了弥补这点缺陷，Java提供了丰富的类库来方便编程者使用，Vector类便是其中之一。事实上，灵活使用数组也可完成向量类的功能，向量类中提供的大量方法也大大方便了用户的使用。
