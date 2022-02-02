 2022年01月25日10:59:36

---

### namespace

1.   有名字的namespace

     ```c++
     1. 
     namespace _name
     {
         // declare variable 
         type val;
     }
     // add prefix when you access it 
     
     _name::val;
     
     
     ```

2.   无名字的namespace 

     ```c++
     2 // you CAN declare a namespace without name for example 
     
     namespace 
     {
     	type val;    
     }
     
     // $$$
     using namespace $$$;
     namespace $$$ 
     {
     	type val;    
     }
     其中这个$$$是在这个名字空间定义所在的作用域里具有的唯一性的名字,不同编译单元里的无名名字空间也不相同. 调用的时候直接使用名字就可以了, 类似全局变量.
         
         
     
     /* */
     ```

     

