# O-RADS + IOTA 계산기

부인과 초음파 난소·부속기 병변을 위한 위험 분류 계산기입니다.

- **O-RADS US v2022** (ACR, 2022년 11월): 점수, 악성 위험도, 권고 관리
- **IOTA Simple Rules**: B/M 소견 기반 양성, 악성, 판정 불가
- **증례 기록**: 두 판정과 병리 결과를 함께 저장, O-RADS × 병리 교차표, CSV 복사

빌드 과정 없는 단일 HTML 파일(`index.html`)입니다. 브라우저로 열면 바로 동작합니다.

## 배포 (GitHub Pages)

1. GitHub에서 새 저장소를 만듭니다. 무료 계정은 Public이어야 Pages를 쓸 수 있습니다.
2. 이 폴더의 파일을 모두 업로드합니다 (Add file → Upload files).
3. Settings → Pages → Build and deployment에서 Source를 `Deploy from a branch`, Branch를 `main` / `(root)`로 선택하고 Save.
4. 1~2분 뒤 `https://<아이디>.github.io/<저장소이름>/`에서 열립니다.

수정할 때는 `index.html`만 바꿔서 다시 올리면 자동으로 반영됩니다.

## 데이터와 개인정보

- 증례 기록은 사용하는 브라우저의 localStorage에만 저장됩니다. 서버로 전송되지 않고, 컴퓨터끼리 동기화되지 않습니다.
- 컴퓨터를 옮길 때는 화면의 **CSV 복사**로 기록을 옮기세요.
- 증례 번호에 이름, 등록번호, 생년월일 등 환자 식별정보를 넣지 마세요.
- `data/` 폴더와 CSV, 엑셀, DICOM 파일은 `.gitignore`로 커밋되지 않게 막아 두었습니다.

## 앞으로 추가할 것

- IOTA ADNEX 모델 (원 논문 계수 대조 후)
- ADNEX 입력 항목 기록 (나이, CA-125, 고형 성분 최대 직경 등)

## 참고 기준

- ACR O-RADS US v2022 Assessment Categories, Classic Benign Lesions
- IOTA Simple Rules (Timmerman et al.)

## 면책

진료 판단을 돕는 참고 도구입니다. 최종 판정과 관리 결정은 영상 소견 전체와 임상 정보를 종합해 전문의가 내려야 합니다.
