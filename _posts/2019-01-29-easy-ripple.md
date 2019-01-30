---
layout: post
title: "[Android] Ripple 효과 쉽게 주기"
categories: Android
---
안드로이드 View에 리플효과 쉽게 주는 방법

1. View의 영역만큼만 리플효과
``` xml
android:background="?selectableItemBackground"
```
``` xml
android:foreground="?selectableItemBackground"
```
``` xml
android:foreground="?selectableItemBackgroundBorderless"
```

2. View를 벗어나며 원형 리플효과
``` xml
android:background="?selectableItemBackgroundBorderless"
```

TIP.
foreground에도 이미지 리소스 넣는 것이 가능하니, 내부가 투명한 프레임 이미지는 백그라운드처럼 사용하면서 원형리플효과를 줄 수 있다.
``` xml
android:background="?selectableItemBackgroundBorderless"
android:foreground="프레임 리소스"
android:padding="2dp"
android:src="이미지 리소스"
```
