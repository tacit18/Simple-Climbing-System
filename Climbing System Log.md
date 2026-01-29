[TOC]

# Climbing System(based on UE5)

## 1.**Basic Climbing Logics and Physics**

### 1)Pre Start: Create a "DebugHelper"

```c++
#pragma once
namespace Debug {
	static void Print(const FString& Msg, const FColor& Color, int Inkey = -1) {
		if (GEngine) {
			GEngine->AddOnScreenDebugMessage(Inkey, 6.f, Color, Msg);
		}
		UE_LOG(LogTemp, Warning, TEXT("%s"), *Msg);
	}
}
```

note:

1. Inkey=-1 Temporary debug messages (won't be updated),while >=0 Update message at that key (replaces).     	

### 2)Climbing Movement

#### Enable climbing（简单逻辑）

按下**“x”键**或者**鼠标中键**，**climb行为启动**（屏幕显示“climb action started.”）

![image-20260129172424086](C:\Users\tacit\AppData\Roaming\Typora\typora-user-images\image-20260129172424086.png)

##### 静态配置

![image-20260129183909934](C:\Users\tacit\AppData\Roaming\Typora\typora-user-images\image-20260129183909934.png)

##### 动态响应(UE平台输入x后)

![image-20260129185549620](C:\Users\tacit\AppData\Roaming\Typora\typora-user-images\image-20260129185549620.png)



##### <u>2026.1.29 </u>conclusion

![image-20260129192056043](C:\Users\tacit\AppData\Roaming\Typora\typora-user-images\image-20260129192056043.png)

------



## **2.Climbing Status**













