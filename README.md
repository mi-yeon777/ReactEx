<<<<<<< HEAD
# ReactEx
리액트 배포 연습& README 작성 연습
=======
# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
>>>>>>> 02a5025 (Initial commit)


# 리액트 bash 배포를 위한 명령어
user@ 내로컬 ~/Desktop/BackEend/React/36.React_File upload_download
내로컬의 프로젝트 경로 지정후

git config --global user.name "na0"(임의)

git config --global user.email "깃허브에 등록된 이메일"

git add .
git commit -m "first commit" (내 커밋 메시지)

깃허브 리포 연결(깃허브에서 새 저장소 만든 뒤 복사)
git remote add origin https://github.com/사용자명/저장소이름.git

푸시(깃허브에 업로드)
git branch -M main
git push -u origin main
