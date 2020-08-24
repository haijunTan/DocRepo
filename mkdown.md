#**Markdown语法**

#1.这是标题

# 一级标题

## 二级标题

### 三级标题

#### 四级标题



#*2.这是斜体*

**这是加粗**

***这是斜体加粗***

~~这是删除线~~

~~***斜体加粗删除线***~~

# 3.这是引用

>asdadf 
>
>>asdf 
>>
>>>Asd
>>>
>>>asdf
>>>
>>>asd 

# 4分割线

-----

*****



# 5图片

![介绍：这是对图片的介绍xxxx。][https://img.iplaysoft.com/wp-content/uploads/2016/typora/typora_banner_2x.jpg"typora好东西 "]

# 6超链接

[Thomas github](https://img.iplaysoft.com/wp-content/uploads/2016/typora/typora_banner_2x.jpg

# 7列表

* 列表1

* 立标2

  1. 列表

  2. 列表2

     a. 列表

     b.  列表

  3. 列表

  4. 列表

     #8表格

     | 姓名 | 性别 | 年龄 |      |      |
     | ---- | ---- | :--- | ---- | ---- |
     | 张三 | 男   | 35   |      |      |
     |      |      |      |      |      |
     |      |      |      |      |      |

     # 9代码

     ```c
     int main(){
       int i;
       printf("test code/n");
       return 0;
     }
     ```

  

# 10流程图

```flow
st=>start: 开始框
e=>end: 结束框
```





# test

```flow
st=>start: 开始框
op=>operation: 处理框
cond=>condition: 判断框
sub1=>subroutine: 子流程
io=>inputoutput: 输入输出框
e=>end: 结束框
st->op->cond
cond(yes)->io->e
cond(no)->sub1(right)->op
```