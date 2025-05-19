# 📁 .github 디렉토리 구성 안내

이 디렉토리는 GitHub 저장소의 **이슈 템플릿**과 **풀리퀘스트(Pull Request) 템플릿**을 정의합니다.  
협업 과정에서 커뮤니케이션을 표준화하여 더 효율적인 개발 환경을 구축할 수 있도록 돕습니다.

---
## 📦 버전 설명

### 1️⃣ `.github/*`
- 모든 파일이 `.md` 형식으로 구성되어 있습니다.

### 2️⃣ `.github_V2/*`
- 이슈는 `.yml` 파일로, PR은 `.md` 파일로 구성되어 있습니다.
- 현재 GitHub에서 `.yml` 형식 이슈 템플릿은 공식 지원하지 않습니다.
- 다운로드 후 `.github_V2` 폴더명을 `.github`로 변경하여 사용하시면 됩니다.
---

## 📂 디렉토리 구조

```
.github
├── ISSUE_TEMPLATE
│   ├── chore_request.yml
│   ├── docs_request.yml
│   ├── empty_request.yml
│   ├── feature_request.yml
│   ├── fix_request.yml
│   ├── refactor_request.yml
│   ├── style_request.yml
│   └── test_request.yml
└── pull_request_template.md
```


---

## 📝 이슈 템플릿 설명

| 파일명 | 설명 |
|--------|------|
| `chore_request.yml` | 운영, 빌드, 의존성 등 유지보수 작업에 대한 이슈 |
| `docs_request.yml` | 문서 작성 및 수정 요청에 대한 이슈 |
| `empty_request.yml` | 분류되지 않은 기타 작업용 이슈 |
| `feature_request.yml` | 새로운 기능 개발 요청 이슈 |
| `fix_request.yml` | 버그 수정 요청 이슈 |
| `refactor_request.yml` | 코드 리팩토링 작업 이슈 |
| `style_request.yml` | 코드 포맷팅, 세미콜론 누락 등 스타일 관련 이슈 |
| `test_request.yml` | 테스트 코드 추가/수정 작업 이슈 |

> 모든 이슈 템플릿은 GitHub에서 `New issue` 클릭 시 자동으로 선택할 수 있습니다.

---

## ✅ Pull Request 템플릿

### ❗주의: GitHub는 PR 템플릿에 `.yml` 형식을 지원하지 않습니다.

- 반드시 `.md` 형식을 사용해야 하며,
- 본 저장소는 `.github/pull_request_template.md` 경로에 템플릿을 작성하여 적용합니다.
- PR 생성 시 자동으로 해당 템플릿이 본문에 삽입됩니다.

### 적용 가능한 경로

GitHub는 다음 위치의 PR 템플릿을 자동 인식합니다:

- `.github/pull_request_template.md` ✅ **(권장 위치)**
- `pull_request_template.md` (루트 디렉토리)

---

## 🛠️ 사용 방법

### 1. 이슈 작성
- GitHub에서 `New issue` 클릭
- 원하는 템플릿 (예: ✨ Feature, 🐛 Fix 등) 선택
- 항목에 맞게 작성

### 2. PR 작성
- 브랜치 푸시 후 `Compare & pull request` 클릭
- 템플릿이 자동 입력됨
- 항목에 맞게 작성 후 제출

---

## 🙋🏻 기타

- 템플릿이 맞지 않거나 새로운 유형이 필요할 경우 `empty_request.yml` 템플릿을 사용해 자유롭게 작성해주세요.
