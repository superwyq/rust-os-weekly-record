第一阶段完成后补一下第一阶段的记录，
首先要吐槽一下第一阶段的readme，流程写的很不清晰，按照流程配置，很容易就翻车配置成了夏季学期的rustlings，看见了群里很多人都在问为什么自己配置好的环境是94道题，原因都是一样的，根据readme配置导致的。
其次自我检讨一下自己学习不够积极，本来几天就能完成的事情，拖到ddl前一天才完成，主要原因还是因为英文书看的太少，遇见全英的流程就发怵，不由自主往后退。
最后总结一下学习rust的心得
## rust是一个什么样的语言，为什么诞生了rust？
每一种语言都有着自己的擅长领域和技术特点，C++ 主打一个自由且底层，Python主打一个生态丰富，极易上手。rust呢？学之前只听说以安全为卖点，具体等到学习了才发现，Rust所谓的以安全为买点的更具体说法应该是：把bug消灭在编译期，在自由和安全之间找到一个平衡点，这就是我对rust的理解和定位。如果说C++ 是无条件相信程序员，那么rust就是无条件不相信程序员，即使程序员声明了unsafe，依旧只是允许程序员执行4种原本不被允许的操作。
至于为什么会有rust，我认为是这是大势所趋，C++正在变得越来越不人不鬼，在引入新特性的同时又要求兼容历史标准，导致现在的C++越来越不够乱，C++需要一个接班的或者说至少是替代项。C和C++作为底层的两个大山，他们的历史太悠久了，从反面来说就是历史包袱太重，很多问题因为兼容历史版本而很难作出有效的解决方案，与其接着对C++进行修修补补，不如直接设计一个新的语言，甩掉历史包袱。

## rust遵循什么编程范式？
rust作为一种新语言，从设计上来讲是多种编程范式混合的，但是从做题和看书的感悟来讲，Rust的整体编程思路是以数据+行为来进行的，舍去了类和继承的概念，进一步减少了耦合，数据与行为进行相互组合，可以通过泛型进行组合，也可以使用闭包进行组合。并且Rust中的宏是非常复杂的，相比于C++的复杂多了，而且Rust的宏并不是像C++一样简单进行文本替换，而是在词法层面进行替换，我们可以使用宏进行编程。总而言之，Rust对各种编程范式的特性进行了合理的支持，想要达到让他们相互配合的程度，我感觉这是异于C++的重要一点，C++的设计思路更像是什么范式都支持，但是对于多种编程范式混用的情况并不如Rust。
## rust中的新特性
rust中新引入的所有权制度，借用制度，以及Option和Result这些特性，刚开始编程不是很适应，感觉处处受牵制，但是用习惯了发现这些特性真的非常有用，有效降低了debug的时间和精力。而且rust的报错信息非常人性，再也不用对着C++的segment error去头疼了。
