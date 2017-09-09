# python
#"Hello world!I 'm going to study python!"
#!/usr/bin/env python
#coding=utf-8
import random
num=random.randint(1,1000)
tries=10
print"请在1到1000之间猜一个数字，你有10次机会"
right=False
while right==False:
    answer=input()
    if answer<num:
        print"太小了"
        tries=tries-1
        print"你还有",tries,"次机会"
    if answer>num:
        print"太大了"
        print"你还有",tries,"次机会"
        tries=tries-1
    if answer==num:
        print"完全正确"
        right=True
    if tries==0:
        print"游戏结束"
        break
