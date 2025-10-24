
# GitHub Pages Starter (Jekyll)

## 1) 이 저장소를 GitHub에 올리기
- 새 저장소 이름을 **{username}.github.io** 로 만들기 (예: `ourjune21.github.io`)
- 이 폴더의 파일을 그대로 push

## 2) GitHub Pages 켜기
- 저장소 → Settings → Pages → Build and deployment: "Deploy from a branch"
- Branch: `main` (또는 `master`), 폴더: `/ (root)`
- 저장 후 1~2분 뒤 `https://{username}.github.io` 접속

## 3) 커스터마이즈
- `_config.yml`의 `title`, `description`, `author` 정보 수정
- `assets/css/style.css`로 스타일 변경
- `_posts`에 새 글 추가: 파일명 `YYYY-MM-DD-title.md`, 상단 Front Matter에 `categories`, `tags` 지정
- 카테고리 페이지 추가하려면 `pages`에 비슷한 형식으로 파일 추가

## 4) 검색
- 헤더 검색창에 입력하면 `/search.json`을 불러 클라이언트에서 필터링합니다(플러그인 불필요).

## 5) 로컬 미리보기(선택)
- Ruby가 있다면: `gem install bundler jekyll` → `bundle init` → `bundle add jekyll` → `bundle exec jekyll serve`
- 하지만 GitHub Pages로 바로 푸시해도 자동 빌드됩니다.
