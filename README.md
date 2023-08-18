# Cnote
### c++引用
1.引用是指针的伪装：
引用&只能引用已经存在的变量，而&本身并不生成一个新的变量
```c++
int a = 5;
int& ref = a;//这个方法创造了别名，ref a 都指向同一个内存地址
```
想要change某个value的值，事实上需要在在相应的内存地址中进行更改
```c++
void Increment(int& value){
  value++;
}
\\创建了一个value的别名，并没有新增内存地址
```
### C++类
面向对象编程
类是将数据和功能组合在一起的一种方法；
创建类的时候可以指定类中内容的可见性，当变量是private时，只有类中的函数才能访问
类创建不了新功能除了使代码保持整洁
```c++
class Player
{
public:
  int x ,y ;
  int speed;
//创建函数 如果需要调用class的内容，不用再传参
  void Move(int xa,int ya){
     x =、、、；
     y = 、、、；
}
};

//调用
Player p;
p.move(a,b); 
```
### class类与struct结构体的区别
基本上没有什么区别只有关于可见度上的：类默认成员是private的，struct默认成员是public的；
struct保留下来就是为了保持和C的兼容性。
用class来继承；

### 如何写一个类class
```c++
class log
{
};
```
