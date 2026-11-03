# agent_core

이 폴더는 보안 에이전트 개발을 위한 파이썬 기초 문법 및 실습 코드를 관리하는 공간입니다.  
현재 폴더 내의 `.py` 파일들을 기반으로 학습 중인 내용과 각 파일의 상세 역할을 정리했습니다.

---

## 1. 현재 배우는 내용

- **조건문 분기 (`if`, `else`)**:
  - 점검 결과(`SUCCESS`, `FAIL`, `OK`)에 따른 분기 처리
  - 수치 비교 연산자(`>=`)를 이용한 임계치 판단 ("추가 확인", "기록 유지")
- **리스트(List) 자료형 다루기**:
  - 계정 목록 리스트 생성 및 인덱싱(`users[0]`), 길이 확인(`len()`), 요소 추가(`append()`)
- **반복문 (`for`)**:
  - `for ... in ...` 구문을 통한 리스트 요소 순회 및 출력
  - `range()` 함수를 활용한 정해진 횟수 반복 제어
  - f-string(`f"{number + 1}번째 점검"`)을 이용한 회차별 포맷 출력
- **외부 패키지 점검 (`import`)**:
  - 보안 점검 및 HTTP 통신에 자주 사용되는 `requests` 모듈 로드 및 버전 확인

---

## 2. 실제 만든 파일 목록 (`.py`)

| 파일명 | 학습 및 코드 내용 |
| :--- | :--- |
| [`assignment_02_f1.py`](./assignment_02_f1.py) | **조건문 기초 (문자열 비교)**<br>- `result` 변수 값이 `"FAIL"`인지 비교하여 `"확인 필요"` / `"점검 대상"` / `"계속 진행"` 출력 분기 실습 |
| [`assignment_02_f2.py`](./assignment_02_f2.py) | **비교 연산자 및 상태 판별**<br>- `count >= 3` 조건을 통해 `"추가 확인"` 또는 `"기록 유지"` 출력<br>- `result == "OK"` 조건을 통해 `"정상"` 또는 `"실패"` 출력 |
| [`assignment_03_f1.py`](./assignment_03_f1.py) | **리스트와 for 반복문**<br>- 계정 목록(`users`) 리스트 생성<br>- `for user in users:` 구문으로 전체 사용자 계정 순회 및 출력 |
| [`assignment_03_f2.py`](./assignment_03_f2.py) | **range() 함수를 활용한 반복문 실습**<br>- `range(1, 4)`를 통해 1부터 3까지 출력하며 종료 조건(stop 미포함) 확인<br>- `range(5)`와 f-string을 활용해 `1번째 점검` ~ `5번째 점검` 메시지 출력 |
| [`check_requests.py`](./check_requests.py) | **외부 라이브러리 확인**<br>- `import requests`를 통해 패키지 정상 로드 여부 및 `requests.__version__` 출력 |

---

## 3. 실행 방법

각 파이썬 파일은 터미널에서 다음과 같이 실행할 수 있습니다:

```bash
python assignment_02_f1.py
python assignment_02_f2.py
python assignment_03_f1.py
python assignment_03_f2.py
python check_requests.py
```
