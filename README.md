# xconda-planning

XCONDA 기획 산출물 전용 레포. 개발 코드는 [xconda-board](https://github.com/hanahchafilmaker/xconda-board)에 있고, 여기는 기획 문서와 결정·추적만 둔다.

- 운영 시트: [XCONDA_운영서버_개발실행시트_v0.3_20261113](https://docs.google.com/spreadsheets/d/19XTjmufejkJixSuMww5R4GmfMwoHpgooWy49HQhReiE/edit) (구글 시트가 원본, 13탭, 이 레포는 산출물 보관·추적용)
- 스킬: planning-docs-kit v1.1.0 (요구사항 정의서 → 기능 명세서 → 화면 설계서 → QA 테스트 시트 → WBS, 같은 REQ ID로 연결)
- 대시보드 (GitHub Pages): [기획 대시보드](https://hanahchafilmaker.github.io/xconda-planning/) · [마케팅 대시보드](https://hanahchafilmaker.github.io/xconda-planning/marketing/)

## 구조

| 경로 | 내용 |
|---|---|
| `docs/01-requirements/` | 요구사항 정의서 (REQ) |
| `docs/02-features/` | 기능 명세서 (FNC) |
| `docs/03-wireframe/` | 화면 설계서 (SCR) |
| `docs/04-qa/` | QA 테스트 시트 (TC), 버그 리포트 |
| `docs/05-wbs/` | WBS, 간트 |
| `docs/06-trace/` | 추적 매트릭스, 릴리스 체크리스트, 현황 스냅샷 |

## ID 체계

- 요구사항 `REQ-<영역>-<3자리>` / 기능 `FNC-<영역>-<3자리>` / 화면 `SCR-<영역>-<3자리>` / 테스트 `TC-<영역>-<3자리>` / 작업 `W-<3자리>`
- 단, 블로킹보드 운영 시트는 기존 번호(`FR-01~24`, `NFR-01~09`, 기능 `0-01~6-15`, WBS `1.1`식)를 쓰고 있어 이 레포로 옮길 때 매핑표가 필요하다. 매핑 없이 번호를 새로 매기지 않는다.
- 없는 수치·기한은 지어내지 않고 `확인 필요`로 표시한다.

## 현황 (v0.3 기준, 2026-11-13)

- 요구 46건 (FR 33 + PAY 7 + TRN 6), 기능 74건, WBS 13.25MD (전유준 7.25 / 권태윤 3.75 / 공동 1.75 / 차하나 PM 0.5)
- QA TC 74건 (판정 전부 미실행), 커버리지 87% (40/46), 미결 31건 (결정 8 + 기능 7 + 실행 16)
- 결-1~8: 확정안 8/8 공란, 기한 2026-11-16, 관련 TC 22건
- 일정: 11/16(월) 결정 확정 마감 → 11/17(화) test 배포·TC 실행 → 11/18(수) 운영 배포. 차단 조건 PAY-E2E 미통과 (TC-PAY-005)
- UIUX 개편 보류 (2026-11-13): T-53~T-61·T-63 보류, T-62 중단

## 주의

- 이 레포는 public이다. 내부 문서(태스크 파일 등 내부 수치 포함)는 올리지 않는다.
- Pages는 내보낸 시점 기준 스냅샷이라 대시보드가 바뀌면 다시 내보내서 푸시해야 한다.
