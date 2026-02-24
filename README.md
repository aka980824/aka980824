<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=soft&color=3561f1&height=180&text=JaeWoo%20Park&animation=scaleIn&fontColor=000000&fontSize=70" />
</div>

<div align="center">

### Web Developer · Collaboration · Quality Mindset

<b>“끝까지 완성하고, 문제를 원인부터 고쳐서 안정화하는” 개발자 박제우입니다.</b><br/>
일정·할 일·채팅·커뮤니티를 하나로 통합한 웹 서비스 <b>Planix</b>를 팀장으로 개발하며<br/>
기획 → 설계 → 구현 → 협업 → 버그 분석/개선까지 전 과정을 경험했습니다.

<br/>

<a href="https://teamppro.github.io/totalproject/main">
  <img src="https://img.shields.io/badge/Planix%20Live%20Demo-3561f1?style=for-the-badge&logo=vercel&logoColor=white"/>
</a>
<a href="https://github.com/TeampPro/totalproject?tab=readme-ov-file">
  <img src="https://img.shields.io/badge/Planix%20Repo-181717?style=for-the-badge&logo=github&logoColor=white"/>
</a>
<a href="mailto:aka980824@naver.com">
  <img src="https://img.shields.io/badge/aka980824@naver.com-03C75A?style=for-the-badge&logo=naver&logoColor=white"/>
</a>

</div>

---

## ⭐ Featured Project | Planix

<div align="center">
  <img width="900" alt="Planix Banner" src="https://github.com/user-attachments/assets/b5776483-2f7c-498f-a9ca-155db3dca544" />
</div>

**Planix**는 캘린더/투두/메신저가 분리되어 협업 시 일정·할 일 파악이 어려운 문제를 해결하기 위해  
**“일정 · 할 일 · 채팅”을 한 화면에서 통합 관리**하도록 설계한 협업 서비스입니다.

- **기간**: 2025.10.29 ~ 2025.12.10  
- **역할**: 팀장(기획/기능 정의/일정 관리/협업 운영/핵심 기능 구현)
- **핵심 포인트**: *실시간 채팅(WebSocket) + 캘린더 Drag&Drop + 공유 일정 + 커뮤니티/관리자*

---

## 🖼️ Screenshots & Feature Highlights

> ✅ 아래 GIF/이미지 링크는 `TeampPro/totalproject` 레포의 `assets` 경로를 기준으로 작성했습니다.  
> 만약 폴더명이 다르거나 대소문자가 다르면, 해당 경로만 실제 레포에 맞게 바꿔주면 돼요.

<table>
  <tr>
    <td align="center"><b>Main Dashboard</b></td>
    <td align="center"><b>Calendar CRUD</b></td>
    <td align="center"><b>Drag & Drop</b></td>
    <td align="center"><b>Chat (WebSocket)</b></td>
  </tr>
  <tr>
    <td><img src="https://raw.githubusercontent.com/TeampPro/totalproject/main/assets/MainPage.gif" height="150"/></td>
    <td><img src="https://raw.githubusercontent.com/TeampPro/totalproject/main/assets/Add.gif" height="150"/></td>
    <td><img src="https://raw.githubusercontent.com/TeampPro/totalproject/main/assets/DragDrop.gif" height="150"/></td>
    <td><img src="https://raw.githubusercontent.com/TeampPro/totalproject/main/assets/ChatPage.gif" height="150"/></td>
  </tr>
</table>

<table>
  <tr>
    <td align="center"><b>Share Schedule</b></td>
    <td align="center"><b>Community</b></td>
    <td align="center"><b>Admin</b></td>
    <td align="center"><b>Map / Weather</b></td>
  </tr>
  <tr>
    <td><img src="https://raw.githubusercontent.com/TeampPro/totalproject/main/assets/PublicTodo.gif" height="150"/></td>
    <td><img src="https://raw.githubusercontent.com/TeampPro/totalproject/main/assets/Community.gif" height="150"/></td>
    <td><img src="https://raw.githubusercontent.com/TeampPro/totalproject/main/assets/Admin.gif" height="150"/></td>
    <td>
      <img src="https://raw.githubusercontent.com/TeampPro/totalproject/main/assets/Weather.gif" height="72"/>
      <br/>
      <img src="https://raw.githubusercontent.com/TeampPro/totalproject/main/assets/Map.gif" height="72"/>
    </td>
  </tr>
</table>

---

## 🧠 What I Built (Detail)

### 1) 캘린더/일정 관리
- 일정 **생성/수정/삭제(CRUD)**, Todo 완료 처리
- **Drag & Drop**으로 일정 이동: **시간은 유지하고 날짜만 변경**하는 UX 구현  
- 공유 일정 분리 생성 + D-Day 표시

### 2) 실시간 채팅(WebSocket)
- Spring WebSocket 기반 `/ws/chat` 엔드포인트 구성
- `roomId/memberName` 기반 **입장 검증**, roomId별 세션 관리
- 시스템 메시지 브로드캐스트 + 메시지 DB 저장(재접속 시 조회 가능)

### 3) 커뮤니티/관리자
- 게시글/댓글, 공지 작성
- 관리자 모드(회원/게시글 관리) 구성

---

## 🧩 Problem Solving (대표 이슈 1개로 실력 증명)
**이슈**: Drag & Drop 이후 캘린더는 정상인데 타임라인 막대 위치/길이가 깨짐  
**원인**: startDateTime만 변경되고 endDateTime이 이전 날짜로 남아 **시작/종료 날짜 불일치** 발생  
**해결**: start/end 모두 동일한 새 날짜로 재조합하여 저장 → 타임라인 계산 안정화

---

## 🛠 Tech Stack

<div align="center">
  <img src="https://img.shields.io/badge/Java-007396.svg?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F.svg?style=for-the-badge&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring%20Security-4FA3FF?style=for-the-badge&logo=springsecurity&logoColor=white" />
  <img src="https://img.shields.io/badge/JPA-2F4F4F?style=for-the-badge&logo=hibernate&logoColor=white" />
  <img src="https://img.shields.io/badge/MariaDB-003545.svg?style=for-the-badge&logo=mariadb&logoColor=white" />
  <br/>
  <img src="https://img.shields.io/badge/React-20232a.svg?style=for-the-badge&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/Vite-B3D9FF?style=for-the-badge&logo=vite&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=20232a" />
  <img src="https://img.shields.io/badge/WebSocket-3561f1?style=for-the-badge&logo=socketdotio&logoColor=white" />
</div>

<details>
  <summary><b>📚 More (Tools / Studying)</b></summary>
  <br/>
  <div align="center">
    <img src="https://img.shields.io/badge/Git-F05033.svg?style=for-the-badge&logo=git&logoColor=white" />
    <img src="https://img.shields.io/badge/GitHub-181717.svg?style=for-the-badge&logo=github&logoColor=white" />
    <img src="https://img.shields.io/badge/Sourcetree-0052CC?style=for-the-badge&logo=sourcetree&logoColor=white" />
    <img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white" />
    <img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" />
    <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
  </div>
</details>

---

## 🏅 GitHub Stats 

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=aka980824&theme=tokyonight&no-frame=true&row=1&column=6" />
</div>

---

## 📌 Career Snapshot
- **동우정공(주)**: IATF 16949 인증 취득 실무 총괄(요구사항 분석/문서 표준화/심사 대응)
- **아리모아**: 다수 대학 홈페이지 개발·유지보수(운영 이슈 분석/개선)

---
