# CHANGELOG — Loop Prompt 핸드북

## v1.0.0 — 2026-07-04

### 최초 발행

**대상 버전:** Claude Code 2026.07  
**예시 도메인:** NFC 리드 기반 학급 관리 시스템 설계  
**언어:** 한국어  
**테마:** azure

### 수록 문서

| 파일 | 내용 |
|------|------|
| `docs/index.html` | 랜딩 페이지 (카드 그리드, 사이트 전체 검색) |
| `docs/concepts/Concepts_Chapter.html` | 개념과 원리 (루프 유형 4가지, SELF-REFINE·Reflexion·Meta-Prompting) |
| `docs/tools/Tools_Manual.html` | Claude Code 루프 도구 레퍼런스 (`/loop`, `/goal`, `/schedule`, `ScheduleWakeup`) |
| `docs/tools/Tools_Examples.html` | Claude Code 루프 도구 실습 예시 (초·중·고급 NFC 시나리오 3종) |
| `docs/patterns/Patterns_Manual.html` | 루프 설계 패턴 레퍼런스 (폴링·자기 수정·목표 지향·멀티 에이전트) |
| `docs/patterns/Patterns_Examples.html` | 루프 설계 패턴 실습 예시 (초·중·고급 시나리오 3종) |
| `docs/quiz/Quiz_Quiz.html` | 학습 확인 문제 풀이 (객관식 3·서술형 2·FAQ 5) |

### 주요 설계 결정

- **범위:** Claude Code `/loop`·`/goal`·`/schedule`·`ScheduleWakeup` + 일반 LLM 루프 기법 (SELF-REFINE, Reflexion, Meta-Prompting) 동시 수록
- **300초 함정 명시:** `ScheduleWakeup` 프롬프트 캐시 TTL 경계(300s) 경고를 Tools 매뉴얼과 Quiz에 반복 수록
- **예시 일관성:** 모든 실습 코드·시나리오에 NFC 리드 기반 학급 관리 시스템을 일관 적용
- **정적 배포:** GitHub Pages (main 브랜치 `/docs` 폴더), Jekyll 비활성화(`.nojekyll`)
