# Pointers-BOX 공식 웹사이트

이 저장소는 Pointers-BOX 공식 웹사이트 <https://www.pointers-box.cc.cd> 의 소스 코드입니다. 플랫폼 공지, 버전 업데이트 내역, 클라이언트 다운로드 링크, 사용 안내를 게시합니다.

## 사이트 구성

- **홈 / 소식**: 플랫폼 공지와 일상 소식
- **블로그**: 릴리스 문서와 버전 업데이트 내역(상단 고정)
- **다운로드**: Windows 설치 버전, 포터블 버전, Android 버전 다운로드 링크(GitHub / Gitee / 런저우 클라우드)
- **프로젝트**: Pointers-BOX 클라이언트 소개
- **소개**: 플랫폼 소개, 사용 안내, 커뮤니티 링크

## 기술 스택

- Astro 정적 사이트, 빌드 결과물은 순수 정적 파일
- Svelte 5 컴포넌트 + Tailwind CSS
- 사이트 내 검색은 Pagefind가 빌드 시 인덱스를 생성

## 로컬 실행

요구 사항: Node.js ≥ 22, pnpm 11

```bash
pnpm install
pnpm dev      # 개발 미리보기(기본 http://localhost:4321)
pnpm build    # dist/로 빌드
pnpm preview  # 빌드 결과물 미리보기
```

## 콘텐츠 관리

- **글**: `src/content/posts/*.md`, `pinned: true`로 상단 고정, `pnpm new-post`로 생성
- **소식**: `src/content/dynamic/*.md`, `pnpm new-dynamic`로 생성
- **프로젝트**: `src/content/projects/*.md`
- **사이트 설정**: `src/config/` 아래 페이지별로 분리 — 사이트 정보 `siteConfig.ts`, 내비게이션 `navBarConfig.ts`, 사이드바 `sidebarConfig.ts`, 공지 `announcementConfig.ts`, 배경 `backgroundWallpaper.ts`, 음악 `musicConfig.ts`
- **이미지 및 정적 리소스**: `public/`

## 배포

`pnpm build`로 `dist/` 정적 디렉터리를 생성합니다. 저장소에 푸시하면 호스팅 플랫폼이 자동으로 빌드·배포합니다.

## 링크

- 공식 사이트: <https://www.pointers-box.cc.cd>
- 클라이언트 저장소: <https://github.com/PointersMZX/Pointers-BOX>
- Gitee 미러(릴리스 다운로드): <https://gitee.com/PointersMZX/Pointers-BOX>
- 커뮤니티 QQ 그룹: <https://qm.qq.com/q/DGf5XI9jgW>

## 저작권

© 2026 Pointers-BOX. All Rights Reserved.
