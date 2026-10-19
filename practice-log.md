# 실습 기록

로컬에 저장소를 만들고 파일 다섯 개를 각각 커밋했습니다.
GitHub 저장소를 연결한 뒤 Push했지만 fetch first 오류가 났습니다.
GitHub에서 README와 .gitignore를 먼저 만들어 원격에도 커밋이 있었기 때문입니다.

원격 이력을 가져와 로컬 이력과 합쳤습니다.

```sh
git fetch origin
git merge origin/main --allow-unrelated-histories --no-edit
```

README와 .gitignore에서 충돌이 났습니다.
README는 로컬 설명으로 정리하고, .gitignore는 양쪽 규칙을 합쳤습니다.
수정한 파일을 스테이징하고 병합 커밋을 만든 뒤 다시 Push해 성공했습니다.
