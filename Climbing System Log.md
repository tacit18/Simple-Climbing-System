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

[按下**x键** 或者 **鼠标中键**，**climb行为启动**（屏幕显示“climb action started.”）]https://imgur.com/e5jfihG

##### 静态配置所完成的任务

https://imgur.com/BzvdxvT

##### 动态响应流程(UE平台输入x后)

https://imgur.com/Qm9miot



##### <u>2026.1.29 </u>conclusion

https://imgur.com/eMs6ige



------



## **2.Climbing Status**













