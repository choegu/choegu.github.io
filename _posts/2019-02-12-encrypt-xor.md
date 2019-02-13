---
layout: post
title: "[Android] Encrypt XOR"
categories: Android
---

문자열 encrypt

``` java
public static String encryptXOR(String text, String cipher) {
    char[] key = cipher.toCharArray();

    StringBuilder output = new StringBuilder();

    for(int i = 0; i < text.length(); i++) {
        output.append((char) (text.charAt(i) ^ key[i % key.length]));
    }

    return output.toString();
}
```