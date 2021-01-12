# 期末報告 — 凱撒加密

---
## 摘要
它是一種替換加密的技術，明文中的所有字母都在字母表上向後（或向前）按照一個固定數目進行偏移後被替換成密文。

## 加密
#### 說明:

將字母位移N個位元。

#### 程式

```
def encrypt(input_string: str, key: int, alphabet: Optional[str] = None) -> str:
    alpha = alphabet or ascii_letters
    result = ""
    for character in input_string:
        if character not in alpha:
            result += character
        else:
            new_key = (alpha.index(character) + key) % len(alpha)
            result += alpha[new_key]
    return result
```
#### 結果 
<img src=".\加密.jpg" width = "40%">


## 解密
#### 說明
還原位移量

#### 程式
與加密概念差不多

#### 結果
<img src=".\解密.jpg" width = "40%">

## 參考資料
[https://github.com/TheAlgorithms/Python](https://github.com/TheAlgorithms/Python)
