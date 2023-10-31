# 23b
# C110118215 黃羚蓁
## C110118215 黃羚蓁
### C110118215 黃羚蓁
#### C110118215 黃羚蓁
##### C110118215 黃羚蓁
###### C110118215 黃羚蓁

# :smile:  🚴 

-----

![NKUST](logo.png "NKUST")

----
Emphasis, aka *italics*, with *asterisks* or *underscores*.

Strong emphasis, aka bold, with **asterisks** or **underscores**.

Combined emphasis with **asterisks and underscores.**

Strikethrough uses two tildes. ~~Scratch this:~~

---

1.  First ordered list item
2.  Another item  
  ..* Unordered sub-list.
3.  Actual numbers don't matter,just that it's a number  
    ..1.Ordered sub-list  
    ...2.2nd
4.  And another item.  
  ...*note 1  
  ...*note 2  
  ***note 3  
  
---

- [ ] to do list
- [x] 1st thing
- [ ] 2nd thing
- [ ] 3rd thing
- [ ] 4th thing

---

```python code
s = "python highlighted syntax"
print(s)
```

---
```javascript code
var s = "JavaScript highlighted syntax"
alert(s)
```
---
| Tables | Are | Cool|
| :------------|:-----------:| ------:|
| col 3 is     |right-aligned|   $1600|
| col 2 is     | centered    |     $12|
| zebra stripes| are neat    |      $1|

| Markdown | Less | Pretty|
| :---         |:---        | :---      |
| *Still*      | `renders`  | **nicely**|
| 1            | 2          | 3         |

---
[![Everything Is AWESOME](https://img.youtube.com/vi/StTqXEQ2l-Y/0.jpg)](https://www.youtube.com/watch?v=StTqXEQ2l-Y "Everything Is AWESOME")

---

### 10/31系統分析ZUVIO題目

1.請新增一個CShape的子類別CTriangle，其constructor 共有三個double的參數 a,b,c (為直角三角形的三個邊長)，其面積為0.5*a*b，請寫出CTriangle的類別程式與產生其物件的main 程式(顏色為紅色，a=3, b=4, c=5) 程式碼請放在個人的github 答案請列出其連結

Ans：

**CShape.java**        
~~~
abstract class CShape{
    protected String color;
    public void setColor(String str){
        color = str;
    } 


    public abstract void show();
}
~~~
           
**CTriangle.java**
~~~
class CTriangle extends CShape{
    double ca, cb, cc;
    public CTriangle(double a, double b, double c){
        ca=a;
        cb=b;
        cc=c;
    }
   
    public void show() {
       
        System.out.print("color="+color+"  ");
        System.out.print("area="+0.5*ca*cb);
    }
   
}
~~~
**app11.java**
~~~
public class app11 {
   public static void main(String[] args) {
    CTriangle ct = new CTriangle(3, 4, 5);
    ct.setColor("red");
    ct.show();
}
}
~~~
