# 실습 기록

## 로컬 작업

1. 기존 프로젝트와 분리된 새 폴더를 만듭니다.
2. `git init -b main`으로 저장소를 초기화합니다.
3. 이 저장소에 사용할 커밋 작성자 이름과 noreply 이메일을 설정합니다.
4. README, 제외 규칙, 명령어 정리, 실습 기록, 점검표를 각각 추가하고 커밋합니다.
5. 아래 명령어로 파일 수, 커밋 수, 작업 폴더 상태를 확인합니다.

```sh
git ls-files
git rev-list --count HEAD
git log --oneline
git status --short
```

## GitHub 연결 및 Push

다음은 로컬 작업을 마친 뒤 실행할 절차입니다. 원격 업로드 완료 여부는
`checklist.md`에서 별도로 확인합니다.

1. GitHub에서 이름이 `git-practice`인 Public 저장소를 만듭니다.
2. 로컬 이력을 그대로 올릴 수 있도록 GitHub에서 README 등을 미리 생성하지 않습니다.
3. 아래 주소의 `YOUR_USERNAME`을 실제 GitHub 계정으로 바꿔 실행합니다.

```sh
git remote add origin https://github.com/YOUR_USERNAME/git-practice.git
git push -u origin main
```

4. GitHub 페이지에서 공개 상태, 다섯 파일, 다섯 커밋을 확인합니다.
5. 최종 제출에는 실제 GitHub 저장소의 전체 URL을 사용합니다.
