Interrupt request (PC architecture) 

（重定向自 INTR）

英语百科

####  INTR

>   In a [computer](https://www.frdic.com/dicts/wiki/Computer.html), an interrupt request (or IRQ) is a hardware signal sent to the processor that temporarily stops a running program and allows a special program, an [interrupt handler](https://www.frdic.com/dicts/wiki/Interrupt_handler.html), to run instead. Hardware interrupts are used to handle events such as receiving data from a [modem](https://www.frdic.com/dicts/wiki/Modem.html) or [network card](https://www.frdic.com/dicts/wiki/Network_card.html), key presses, or mouse movements.

#### NMI (Non Maskable Interrupt)——不可屏蔽中断(即CPU不能屏蔽)

不可屏蔽中断请求信号NMI用来通知CPU，发生了“灾难性”的事件，如电源掉电、存储器读写出错、总线奇偶位出错等。NMI线上中断请求是不可屏蔽的（即无法禁止的）、而且立即被CPU锁存。因此NMI是边沿触发，不需要电平触发。NMI的优先级也比INTR高。不可屏蔽中断的类型指定为2，在CPU响应NMI时，不必由中断源提供[中断类型码](https://baike.baidu.com/item/中断类型码/10390216)，因此NMI响应也不需要执行总线周期INTA

​	

![img](https://img-blog.csdnimg.cn/20200421133554420.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyNjA0MTc2,size_16,color_FFFFFF,t_70)