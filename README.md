# Pado 스킬 모음

[Pado](https://github.com/WRL-SPR/pado)가 고른 에이전트 스킬이에요. Claude Code 플러그인 마켓플레이스 형식이라 Pado뿐 아니라 Claude Code에서도 바로 쓸 수 있어요.

## 담긴 것

| 플러그인 | 스킬 | 하는 일 |
|---|---|---|
| korean | korean-ux-writing | 한국어 UI 문구, 오류 메시지, 문서를 자연스러운 해요체로 쓰고 다듬어요 |
| | korean-commit-pr | 한국어 커밋 메시지와 PR 설명을 저장소 형식에 맞춰 써요 |
| | korean-code-review | 심각도 표시와 실패 시나리오를 갖춘 한국어 코드 리뷰를 써요 |
| | korean-privacy-check | 주민등록번호, 연락처, 계좌 같은 개인정보를 다루는 코드를 점검해요 |
| ponytail | (DietrichGebert/ponytail) | 최소 수정과 군더더기 검토 |
| security-audit | (cloudflare/security-audit-skill) | 보안 점검 |

## 쓰는 법

**Pado:** 에이전트 연결 → 찾아보기 → 출처에 `WRL-SPR/pado-skills`를 더해요. 설치할 때 Pado가 스킬 내용을 검사해요.

**Claude Code:**

```
/plugin marketplace add WRL-SPR/pado-skills
/plugin install korean@pado-skills
```

## 라이선스

korean 플러그인의 스킬은 [MIT](LICENSE)예요. ponytail과 security-audit는 각 저장소의 라이선스를 따라요.

## 스킬 더하기

`plugins/<플러그인>/skills/<스킬 이름>/SKILL.md`를 만들고 `.claude-plugin/marketplace.json`의 `skills` 목록에 경로를 더해요. SKILL.md 맨 위에는 `name`과 `description`이 있어야 해요. 실행 파일이나 내려받는 명령은 넣지 않아요.
