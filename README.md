# Patch Annotation Tool


## 설치방법 (Window)


Anaconda 설치

Conda 가상환경 생성
```
conda create --name={가상환경명} python=3.9
conda activate {가상환경명}
```

디렉토리 생성
```
git clone https://github.com/konyul/Patch-Annotation-Tool.git
```


환경 설정
```
cd Patch-Annotation-Tool
pip install -e .
```

명령어 실행 (Patch-Annotation-Tool 외부 폴더에서 실행)
```
labelme
```

## 사용방법 (Window)

1. 좌상단 Open Dir아이콘을 통해 이미지가 존재하는 폴더 업로드
2. CTRL+SHIFT+C 클릭 시 패치 기반 어노테이션 기능 활성화
3. (1,2,3), (q,w) 버튼 클릭 시 클래스 정의 가능

## 기능
1. 패치 갯수 변경 기능 (어플 좌측)
2. 드래그 기능 (Shift 클릭 + 드래그 진행)
3. 실행 취소 기능 (ctrl + z 또는 마우스 Back 버튼), 전체 실행 취소 기능 (U, clean 상태 저장 시 임의 패치 clean으로 annotation 한 후 저장)
4. 파일 이동 기능 (a,d : 이전, 이후)
5. 어노테이션 복사 및 붙여넣기 (현재 프레임에서 ctrl+c -> 이후 프레임에서 ctrl+v, 이미지의 크기가 같은 경우 적용 가능)
6. 어노테이션 패치 제거 기능 (클릭시 x, 드래그시 shift+x)
7. 어노테이션 숨김 기능 (Space 바)
