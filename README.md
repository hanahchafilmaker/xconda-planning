# xconda-planning

XCONDA 기획 산출물 전용 레포. 개발 코드는 [xconda-board](https://github.com/hanahchafilmaker/xconda-board)에 있고, 여기는 기획 문서와 결정·추적만 둔다.

- 운영 시트: [운영 서버 개발 실행 시트](https://docs.google.com/spreadsheets/d/11cBzLOtgakf63jh5BOqLF5j40KFklUMCuHlu8salBII/edit?usp=sharing) (구글 시트가 원본, 이 레포는 산출물 보관·추적용)
- 스킬: planning-docs-kit v1.1.0 (요구사항 정의서 → 기능 명세서 → 화면 설계서 → QA 테스트 시트 → WBS, 같은 REQ ID로 연결)

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

## 현황

- `docs/06-trace/current-state-2026-11-13.md` — 2026-11-13 라이브 점검 기준 현황. FR 33건, 기능 74개, WBS 13.25MD, 결-1~8, QA 시트 없음(TC 0건)이 출발점이다.
