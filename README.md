# pmtrpg Contribution Guide

이 문서에서는 `pmtrpg` 레포지토리를 로컬에 클론(clone)하여 Visual Studio Code(VS Code)를 사용해 기여(contribute)하는 방법을 안내합니다.

---

## 📋 사전 준비

* [**Git**](https://git-scm.com/downloads)이 설치되어 있어야 합니다.
* **Visual Studio Code**가 설치되어 있어야 합니다.
* **GitHub 계정**이 필요합니다.

## 권장

* **Visual Studio Code**에서 **Git Extension Pack**을 **Extensions** 탭에서 **Install** 해두면 편합니다.

---

## 1. 레포지토리 클론(Clone)

1. GitHub 웹사이트에서 레포지토리 페이지(<https://github.com/whitespaca/pmtrpg.md>)를 엽니다.

2. 오른쪽 상단의 **Code** 버튼을 클릭하고, HTTPS 주소를 복사합니다.

   ```text
   https://github.com/whitespaca/pmtrpg.md.git
   ```

3. VS Code를 실행합니다.

4. **Command Palette**를 열려면:

   * Windows/Linux: `Ctrl+Shift+P`
   * macOS: `⌘+Shift+P`

5. `> Git: Clone`을 입력하고 선택합니다.

6. 복사한 URL을 붙여넣고 Enter를 누릅니다.

7. 로컬에 저장할 폴더를 선택하면, VS Code가 자동으로 클론 과정을 수행하고 해당 폴더를 엽니다.

> **팁:** 터미널을 선호한다면, VS Code 내장 터미널(``Ctrl+` ``) 또는 시스템 터미널에서 직접 실행 가능합니다:
>
> ```bash
> git clone https://github.com/whitespaca/pmtrpg.md.git
> code pmtrpg.md
> ```

---

## 2. 새 브랜치(branch) 생성

변경 사항을 안전하게 관리하기 위해, 먼저 새 브랜치를 만듭니다.

```bash
# feature/your-feature-name 대신 기능명을 지정하세요
git checkout -b feature/your-feature-name
```

---

## 3. 코드 수정 및 기능 추가

1. VS Code 파일 탐색기에서 필요한 파일을 열고 수정합니다.
2. 변경사항을 저장(`Ctrl+S` 또는 `⌘+S`)합니다.
3. 새 파일을 추가하거나, 기존 파일을 삭제 및 이동할 때도 동일하게 작업합니다.

---

## 4. 커밋(commit) 및 원격 저장소로 푸시(push)

1. 변경된 파일을 스테이징(stage)합니다:

   ```bash
   git add .
   ```

2. 의미 있는 메시지와 함께 커밋합니다:

   ```bash
   git commit -m "[feat] 새로운 기능 요약 메시지"
   ```

3. 원격(origin)에 브랜치를 업로드합니다:

   ```bash
   git push -u origin feature/your-feature-name
   ```

---

## 5. Pull Request 생성

1. GitHub 웹사이트에서 본인의 브랜치를 확인합니다.
2. **Compare & pull request** 버튼을 클릭합니다.
3. 제목과 설명을 작성하고, 리뷰어를 요청합니다.
4. **Create pull request** 버튼을 누르면 PR이 생성됩니다.

---

## 6. 코드 리뷰 및 병합

* 요청된 리뷰를 확인하고, 피드백을 반영해 커밋을 추가합니다.
* 리뷰어 승인 후, 메인 브랜치에 병합될 수 있습니다.

---

## 7. 기여 가이드라인

* 코드 스타일을 준수해주세요.
* 단위 테스트가 있으면 함께 작성해주세요.
* 새로운 기능은 README나 주석에 문서화해주세요.

---

## 📝 라이선스

이 프로젝트는 [MIT License](LICENSE) 하에 배포됩니다.
