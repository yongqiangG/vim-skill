# vim-skill

## 替换指定字符串

### 全局替换
:%s/旧文本/新文本/g
### 全局替换，但是只替换第一个
:%s/旧文本/新文本/
### 选中替换（visual mode）
:s/就文本/新文本/g
### 指定替换行数
:5,20s/^/#/ （在5-20行行首插入#号）
### 去除行尾空白符
:%s/\s+$//e
### 使用#作为分隔符（避免转义）
:%s#abc/#123/# （将每一行第一个abc/替换成123/）

## 宏的并行执行
1. 选中范围
2. :normal @q （执行q寄存器的宏）
