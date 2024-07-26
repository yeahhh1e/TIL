for문으로 출력 시 자동으로 줄이 바꿔지며 출력 되는 경우가 있음

이 때 **print(string, end="")**으로 입력하면, 문자열만 출력하고 줄 바꿈은 하지 않는다.

(ex)
for i in data_1:
    if i.isupper() == True or i == ' ':
        print(i, end="") # YOU ARE THE BEST