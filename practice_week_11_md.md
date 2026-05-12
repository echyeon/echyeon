# Week 11 실습

## 오늘 한 것
- PyInstaller 설치 및 빌드
- resource_path() 함수 추가
- `--add-data` 옵션으로 에셋 포함
- `.exe` 실행 확인

---

## resource_path() 를 써야 하는 이유

PyInstaller로 exe 파일을 만들면 프로그램이 임시 폴더에서 실행되기 때문에 기존 상대경로로는 이미지나 사운드 파일을 찾지 못하는 문제가 발생한다.  
이를 해결하기 위해 `resource_path()` 함수를 사용하여 실행 환경에 맞는 경로를 자동으로 불러오도록 수정하였다.

---

## 빌드 명령어

```bash
py -m PyInstaller --onefile --add-data "SOUND;SOUND" --add-data "good;good" --add-data "*.png;." main.py
```

---

## AI 활용 내역

ChatGPT를 활용하여 PyInstaller 설치 방법, exe 빌드 과정, 상대경로 오류 해결 방법, `resource_path()` 함수 작성 방법 등을 학습하고 문제 해결에 활용하였다.

