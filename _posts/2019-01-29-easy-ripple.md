---
layout: post
title: "Android Ripple 효과 쉽게 주기"
categories: Android
---
안드로이드 View에 리플효과 쉽게 주는 방법

1. View의 영역만큼만 리플효과
~~~ xml
android:background="?selectableItemBackground"
~~~
~~~ xml
android:foreground="?selectableItemBackground"
~~~
~~~ xml
android:foreground="?selectableItemBackgroundBorderless"
~~~

2. View를 벗어나며 원형 리플효과
~~~ xml
android:background="?selectableItemBackgroundBorderless"
~~~


간혹 background에 리소스가 들어간 상태로 원형리플효과가 필요할 때가 있는데, 그 때 사용할 수 있는 방법 아시는 분은 알려주시면 감사하겠습니다.