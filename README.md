# Patch Annotation Tool


## 설치방법 (Window, Linux)


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

## 사용방법 

1. 좌상단 Open Dir 아이콘을 통해 이미지가 존재하는 폴더 업로드
2. ctrl+shift+c 클릭 시 패치 기반 어노테이션 기능 활성화
3. (1,2,3), (q,w) 버튼 클릭 시 클래스 정의 가능 (1 : 물방울, 2 : 먼지, 3 : 벌레, q : blur, w : blockage), 현재 물방울의 경우만 데이터에 포함
4. ctrl+s 클릭 시 해당 어노테이션 저장 (json 형태로 동일 폴더 내 저장)
5. a,d 버튼 클릭 시 파일 이동

## 기능
1. 드래그 어노테이션 기능 (Shift 클릭 + 드래그 진행)
2. 어노테이션된 패치 취소 기능 (x + 클릭, 또는 shift + x + 드래그)
3. 실행 취소 기능 (ctrl + z) -> 저장하지 않는 경우에만 사용 가능
4. 전체 실행 취소 기능 (u, clean 상태 저장 시 임의 패치 clean으로 annotation 한 후 저장) -> 저장하지 않는 경우에만 사용 가능
5. 이미지 별 어노테이션 복사 및 붙여넣기 (현재 프레임에서 ctrl+c -> 이후 프레임에서 ctrl+v, 이미지의 크기가 같은 경우에만 적용 가능)
6. 어노테이션 숨김 기능 (Space 바)
7. 우측 하단 파일리스트의 체크표시를 통해 어노테이션 상황 파악 가능
8. 패치 갯수 변경 기능 (어플 좌측) (현재는 사용할 필요 없는 기능)
