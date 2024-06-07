conda create --name=labelme python=3

conda activate labelme

가상환경의 site-packages 안에 git clone

제 로컬 예시   ->     C:\Users\LDY\anaconda3\envs\labelme\Lib\site-packages\labelme

https://pypi.org/project/labelme/ 여기에서 tar 파일 다운로드를 받고 

tar -xvf labelme-5.4.1.tar.gz 해서 로컬의 원하는 위치에 압축을 풀고

setup.py파일에서 아래 함수와 같이 encoding='utf-8'을 추가

```
def get_long_description():
    with open("README.md", encoding='utf-8') as f:
        long_description = f.read()
    return long_description
```

labelme 가상환경 activate 후

그리고 labelme-5.4.1파일로 들어가서 pip install -e . 로 설치해주면 해결됩니다.





사용법

1. 설치 후 anaconda 가상환경 실행 후 ->  labelme실행

  (labelme) D:\project\labelme-5.4.1>labelme

2. 좌상단 open 아이콘 클릭 후 원하는 파일 실행 

3. ctrl+shift+c (제가 임의로 지정) 후 클릭 후 곡선 마음대로 그리고 enter키

  class1(초록색) / class2(빨간색) /class3(파란색) 원하는 걸로 입력


____________________________________________________________________________________________
추가된 사용방법

곡선을 그린후에 엔터를 누르고 1w 3r 3q 같이 입력 혹은 clear로 바꾸고 싶다면 00 입력

class는 1,2,3 -> 1,2,3

BLUR는 q,w,e,r -> 1,2,3,4

사용가능합니다

그리고 현재 만든 GT는 Prompt에서 지속적으로 볼 수 있습니다.

Json파일 안에 "label"에 16x16의 list안에 [class, blur] 형태로 저장이 됩니다.
