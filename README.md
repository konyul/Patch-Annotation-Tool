# Patch Annotation Tool


## 설치방법 (Window)


Anaconda 설치

Conda 가상환경 생성
```
conda create --name={가상환경명} python=3
conda activate {가상환경명}
```

디렉토리 생성
```
git clone https://github.com/konyul/Pixel-Annotation-Tool.git
```


환경 설정
```
cd Pixel-Annotation-Tool
pip install -e .
```

명령어 실행 (Pixel-Annotation-Tool 외부 폴더에서 실행)
```
labelme
```

## 사용방법 (Window)

1. 좌상단 Open 아이콘을 통해 이미지 업로드
2. CTRL+SHIFT+C 클릭 시 패치 기반 어노테이션 기능 활성화
3. (1,2,3,4), (q,w) 버튼 클릭 시 클래스 정의 가능
