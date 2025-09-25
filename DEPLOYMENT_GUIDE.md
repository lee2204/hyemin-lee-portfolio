# 🚀 이혜민 포트폴리오 배포 가이드

## GitHub + Vercel 배포 단계별 가이드

### 1단계: GitHub 리포지토리 생성

1. [GitHub.com](https://github.com)에 로그인
2. **"New repository"** 버튼 클릭
3. Repository name: `hyemin-lee-portfolio`
4. **Public**으로 설정
5. **"Create repository"** 클릭

### 2단계: 로컬에서 GitHub에 푸시

아래 명령어들을 순서대로 실행하세요:

```bash
# 원격 저장소 추가 (YOUR_USERNAME을 실제 GitHub 사용자명으로 변경)
git remote add origin https://github.com/YOUR_USERNAME/hyemin-lee-portfolio.git

# main 브랜치로 이름 변경
git branch -M main

# GitHub에 푸시
git push -u origin main
```

### 3단계: Vercel에서 배포

1. [Vercel.com](https://vercel.com)에 접속
2. **GitHub 계정으로 로그인**
3. **"Add New"** → **"Project"** 클릭
4. **"Import Git Repository"** 섹션에서 방금 생성한 `hyemin-lee-portfolio` 리포지토리 선택
5. **"Import"** 클릭
6. 프로젝트 설정:
   - **Project Name**: `hyemin-lee-portfolio`
   - **Framework Preset**: `Other` (기본값 유지)
   - **Root Directory**: `./` (기본값 유지)
   - **Build Command**: 비워둠
   - **Output Directory**: 비워둠
   - **Install Command**: 비워둠
7. **"Deploy"** 버튼 클릭

### 4단계: 배포 확인

- 배포 완료 후 Vercel이 제공하는 URL (예: `https://hyemin-lee-portfolio.vercel.app`)에 접속
- 포트폴리오가 정상적으로 표시되는지 확인

## 🔄 자동 배포 설정 완료!

이제 GitHub 리포지토리에 코드를 푸시할 때마다 Vercel이 자동으로 새 버전을 배포합니다.

## 📝 추가 설정 (선택사항)

### 커스텀 도메인 연결
1. Vercel 프로젝트 대시보드에서 **"Settings"** → **"Domains"**
2. 원하는 도메인 입력 후 DNS 설정

### 환경 변수 설정
1. Vercel 프로젝트 대시보드에서 **"Settings"** → **"Environment Variables"**
2. 필요한 환경 변수 추가

## 🛠️ 문제 해결

### 이미지가 표시되지 않는 경우
- 한글 폴더명으로 인한 경로 문제일 수 있습니다
- 모든 이미지 파일이 올바르게 업로드되었는지 확인하세요

### 404 오류가 발생하는 경우
- `vercel.json` 파일이 올바르게 설정되어 있는지 확인하세요
- 파일 경로가 대소문자를 구분하므로 정확한지 확인하세요

## ✨ 배포 완료!

배포가 완료되면 다음과 같은 URL을 받게 됩니다:
`https://hyemin-lee-portfolio.vercel.app`

이 URL을 통해 전 세계 어디서나 포트폴리오에 접근할 수 있습니다!