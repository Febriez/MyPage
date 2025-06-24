# 옥병준 | 풀스택 개발자

> **LLM 프롬프트 엔지니어링과 백엔드 개발을 통한 창의적 문제 해결 능력을 보유한 풀스택 개발자**

📧 febrie@naver.com | 📱 +82 세부 연락처는 E-Mail 로 요청 바랍니다 | 🔗 [GitHub](https://github.com/Febriez?tab=repositories)

## 💡 핵심 역량

- Java 기반 백엔드 서버 설계 및 구현 능력
- LLM(Claude) API를 활용한 프롬프트 엔지니어링으로 **토큰 사용량 70% 절감**
- 외부 API 연동 및 비동기 처리 시스템 구축 경험
- Unity 클라이언트 UI 개발 참여 경험

## 🛠️ 기술 스택

### 백엔드 개발
![Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white)
![Undertow](https://img.shields.io/badge/Undertow-4E7896?style=for-the-badge&logo=jboss&logoColor=white)
- **주요 기술**: Java, Undertow, OkHttp, Gson
- **비동기 처리**: ExecutorService, CompletableFuture

### AI/LLM
![Claude](https://img.shields.io/badge/Claude_API-7C3AED?style=for-the-badge&logo=anthropic&logoColor=white)
- **Anthropic Claude API**
- **프롬프트 엔지니어링**
- **JSON 스키마 설계**
- **토큰 최적화**

### 외부 API 연동
- **Meshy AI API**
- **RESTful API**
- **비동기 처리**
- **폴링 시스템**

### 프론트엔드/게임 개발
![Unity](https://img.shields.io/badge/Unity6-000000?style=for-the-badge&logo=unity&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)

## 📁 프로젝트

### E-Room: AI 기반 3D 방탈출 게임 자동 생성 시스템
**기간**: 2024.05 - 2024.07 | **팀 규모**: 6명

**프로젝트 개요**: Unity6 기반 3D 방탈출 게임에서 플레이어의 입력(테마, 키워드)을 바탕으로 시나리오, 3D 모델, 게임 스크립트를 완전 자동으로 생성하는 시스템 개발

#### 👨‍💻 담당 역할
- **백엔드 서버 개발** (90%)
- **프롬프트 엔지니어링** (100%)  
- **Unity UI 개발** (30%)

#### 📌 주요 개발 내용

##### 1. 백엔드 서버 아키텍처 설계 및 구현

**비동기 요청 처리 시스템 구축**
- Undertow 서버 기반 RESTful API 설계
- `ExecutorService`와 `CompletableFuture`를 활용한 병렬 처리 구현
- 요청 큐잉 시스템으로 동시 요청 관리 (`BlockingQueue` 활용)

**다중 API 통합 관리**
- **Anthropic Claude API**: 시나리오 및 스크립트 생성
- **Meshy AI API**: 3D 모델 생성 (preview → refine 2단계 처리)
- **로컬 모델 서버**: 라운드 로빈 방식의 부하 분산

##### 2. LLM 프롬프트 엔지니어링

> 🎯 **핵심 성과**: 프롬프트 최적화를 통해 **2,500자 → 750자 (70% 압축)** 달성

**명시적 제약 조건 설계**
```
"ALL existing_objects MUST keep their EXACT original names"
```
- 기존 객체명 불변 규칙 적용
- 참조 무결성 확보로 서버 파싱 오류 제거

**조건부 로직 구현**
- 무료/유료 모델링 모드 분기 처리
- `is_free_modeling` 플래그에 따른 동적 프롬프트 변경

**출력 형식 강제**
- 엄격한 JSON 스키마 준수 (model_scales 단일값 반환 등)
- 한국어/영어 혼용 규칙 정립 (Debug.Log만 한국어)

##### 3. 기술적 문제 해결

**대용량 응답 처리 최적화**
- 오브젝트 10개 이상 시 배치 처리 도입 (5개씩 분할)
- GameManager 의존성 해결을 위한 순차적 생성 전략

**3D 모델 폴리곤 최적화**
- 32만개 → **32,768개 (2^15)** 제한으로 성능 개선
- GPU 친화적 구조로 렌더링 최적화

**에러 처리 및 모니터링**
- 상세한 로깅 시스템 구현 (요청/응답 전체 저장)
- 타임아웃 및 폴링 실패 대응 로직

##### 4. Unity 클라이언트 UI 개발
- 방 생성 요청 UI 컴포넌트 설계 및 구현
- 실시간 생성 상태 표시 시스템
- 서버 응답에 따른 동적 UI 업데이트

#### 🔧 사용 기술
`Java` `Undertow` `Claude API` `Meshy AI API` `Unity6` `C#` `JSON` `RESTful API`

---

## 🎓 교육
*추후 작성 예정*

## 🏆 자격증 및 기타
*추후 작성 예정*
