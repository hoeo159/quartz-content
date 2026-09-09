---
title: build
tags:
  - quartz
created: 2026-09-07
---


테스트는 wsl 터미널에서 `npm run site:serve`로 로컬 미리보기
한번만 빌드하려면 `npm run site:build`

발행은 
`cd /mnt/d/github/my/quartz-content`
`git add -A && git commit -m "새 글: 제목" && git push`
아니면 그냥 github desktop 쓰기

사이트 설정은 quartz.config.yaml
v5를 main branch로 관리하기

Quartz update
```
cd ~/github/my/quartz
git fetch upstream
git merge upstream/v5
npm install && npm run install-plugins
npm run site:serve        # 깨진 곳 없는지 확인 후 push
```

