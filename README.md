# ATmega32U4--1.6--Timer-Application-
用Timer，让一个LED 0.3s内到达最亮，然后再用0.6秒熄灭。模拟心脏的跳动。
####  电路图  
![695225563352722851](https://github.com/wenxiwei00/ATmega32U4--1.4--Timer2/assets/114196821/adbdb2fa-d7a5-402b-97ab-48bd1e391e8f)  
注意这里一定要用PC6口才可以，因为我的代码里面用到了OCR3A寄存器，只有PC6与OCR3A关联  
<img width="474" alt="40b7affe50dca9e6497f2fd98db97e3" src="https://github.com/wenxiwei00/ATmega32U4--1.4--Timer2/assets/114196821/13a6e06d-37fe-4839-b3e1-d59b9d8f8c29">
####  最终效果  
通过调整main.c里面的void heartbeatPattern(void)，可以调整小灯到最亮以及熄灭的时间  
最终效果也可以在youtube上查看：https://youtu.be/R2LBFy5sQ2o  
####  参考资料  
可以找到如何设置Timer mode，如何设置pre-scaler...  
https://medesign.seas.upenn.edu/index.php/Guides/MaEvArM-timer3
