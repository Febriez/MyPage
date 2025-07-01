# 옥병준 | 풀스택 개발자 (Backend & AI 중심)

📧 febrie@naver.com  
📱 연락처는 E-Mail로 요청 바랍니다  
🔗 [GitHub](https://github.com/Febriez?tab=repositories)

> **LLM 프롬프트 엔지니어링과 Java 백엔드 아키텍처 설계에 강점을 가진 창의적 문제 해결형 개발자**

---

## 💡 핵심 역량

- Java 기반 서버 아키텍처 설계 및 비동기 처리 시스템 구현
- LLM 프롬프트 엔지니어링을 통한 **토큰 사용량 70% 절감**, **응답 속도 70% 개선**
- Claude/Meshy 등 외부 AI API 통합 및 오류 회복 설계 경험
- Unity6 기반 클라이언트와의 실시간 통신 및 UI 개발

---

## 🛠️ 기술 스택

**Backend**  
`Java`, `Undertow`, `OkHttp`, `Gson`, `ExecutorService`, `CompletableFuture`  
- RESTful API 설계, 비동기 요청 처리, API 통합 모듈화

**AI / LLM**  
`Claude API`, `Meshy API`, `Prompt Engineering`, `Token Optimization`, `JSON Schema Design`  
- 토큰 최적화, 출력 구조 강제, 조건부 프롬프트 제어

**Frontend / Game**  
`Unity6`, `C#`, `UI Toolkit`, `실시간 상태 표시`, `서버-클라이언트 연동`

**협업 및 문서화**  
`Git`, `GitBook`, `Mermaid`, `Notion`

---

## 📁 프로젝트 경험

### 🎮 E-Room – AI 기반 방탈출 게임 자동 생성 시스템
**2024.05 ~ 2024.07 / 팀 프로젝트 / 담당 비중 90% 이상**

Unity6 기반 3D 방탈출 게임에서 플레이어의 입력을 바탕으로, Claude와 Meshy API를 활용해 시나리오, 스크립트, 3D 모델을 자동 생성하는 시스템을 구축했습니다.

#### ✅ 주요 기여

**1. 백엔드 서버 개발**
- Undertow 기반 REST API 서버 아키텍처 설계 및 구현
- **비동기 병렬 처리 시스템** (ExecutorService, CompletableFuture) 구축
- Claude, Meshy, 로컬 모델을 **모듈화된 인터페이스로 통합**하여 유지보수성 확보
- **Tracking ID 반환 → 클라이언트는 결과 Polling** 방식 설계로 UX 개선

**2. 프롬프트 엔지니어링**
- 토큰 최적화: **2,500자 → 750자 (70% 절감)**  
- 명시적 제약 조건 및 JSON 출력 포맷 강제  
- `is_free_modeling` 등 조건 기반 분기 처리로 **단일 프롬프트 다형성 구현**

**3. 기술 최적화 및 문제 해결**
- Claude 응답 시간 **2분 40초 → 50초 (70% 단축)**  
- 대용량 3D 요청을 **5개 단위로 배치 처리**하여 성능 안정화  
- **32만 폴리곤 → 32,768 (2^15) 제한 최적화**로 GPU 성능 개선  
- 로깅 시스템 및 폴링 실패 대응 로직 구현

**4. Unity UI 개발**
- 방 생성 UI 및 생성 상태 실시간 표시 컴포넌트 개발  
- 서버 응답에 따른 동적 UI 반영 및 유효성 검증 로직 작성

#### 🔧 사용 기술  
`Java`, `Undertow`, `Claude API`, `Meshy API`, `ExecutorService`, `CompletableFuture`, `Unity6`, `C#`, `JSON`, `RESTful API`, `GitBook`, `Mermaid`

---

## 🎓 교육
- 하이미디어아카데미: 심화_생성형 AI활용 인재양성과정 (조별멘토)

## 🏆 자격증 및 기타
- SW코딩자격1급
