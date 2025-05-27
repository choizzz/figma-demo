# figma-demo
 - React 19.1.0

# 소스 저장소
 - https://github.com/choizzz/figma-demo-src
   
# 배포 URL
 - https://choizzz.github.io/figma-demo/

# 로컬 실행 방법
1. https://github.com/choizzz/figma-demo-src 에서 소스 내려받기
2. 라이브러리 설치
    ```
    npm install react react-dom redux react-redux react-router-dom bootstrap react-bootstrap react-icons @reduxjs/toolkit
    ```
3. 개발서버 실행
   ```
   npm run dev
   ```
4. 브라우저에서 접근 확인
   ```
   http://localhost:5173/figma-demo
   ```

# 주요 기능 구현 방식
 - Redux Toolkit을 사용하여 캔버스 내 데이터를 전역으로 관리
 - Router를 사용하여 Path Parameter 사용
 - React-Bootstrap을 사용하여 대중적인 UI 사용
 - 로컬 스토리지 기반으로 데이터 저장 / 불러오기 기능 구현
 - 캔버스 내 위치한 도형을 더블클릭하여 속성 편집 가능
   
# 추가적인 구현방식
1. Undo, Redo
   - 이벤트 단위로 스택에 state를 기록하여 되돌리기, 되살리기 기능 구현
     
2. 데이터 공유
   - 현재 캔버스 내 state를 base64문자열로 외부로 전달 가능
   - 공유 받은 사용자는 Path Parameter로 사용하여 바로 데이터 확인가능
   - ex) https://choizzz.github.io/figma-demo/#/eyJjb21wb25lbnRzIjpbeyJpZCI6MTc0ODMyNzc0NTcxNCwidHlwZSI6InNxdWFyZSIsIngiOjMyMiwieSI6MjQyLCJ3aWR0aCI6MTAwLCJoZWlnaHQiOjEwMCwidGV4dCI6IiIsImJhY2tncm91bmRDb2xvciI6IiM5ZTllOWUiLCJmb250Q29sb3IiOiIjZmZmIn0seyJpZCI6MTc0ODMyODY0NTc4OCwidHlwZSI6InNxdWFyZSIsIngiOjE4MywieSI6MTEwLCJ3aWR0aCI6MTAwLCJoZWlnaHQiOjEwMCwidGV4dCI6IiIsImJhY2tncm91bmRDb2xvciI6IiM5ZTllOWUiLCJmb250Q29sb3IiOiIjZmZmIn0seyJpZCI6MTc0ODMyODY3MzUyMywidHlwZSI6InRleHQiLCJ4Ijo1NDAsInkiOjE3NCwid2lkdGgiOjEwMCwiaGVpZ2h0Ijo1MCwidGV4dCI6Iu2FjeyKpO2KuCIsImJhY2tncm91bmRDb2xvciI6IiM5ZTllOWUiLCJmb250Q29sb3IiOiIjZmZmIn1dLCJjYW52YXNTaXplIjp7IndpZHRoIjoiMTgwMCIsImhlaWdodCI6IjEyMDAifX0=
