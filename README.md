# amplify-math

Amplify Classroom(Desmos)의 메모·수식 답변·CL에 들어갈 수학 수식을 작성·검수·변환하는 스킬입니다.

Amplify의 수식은 표준 LaTeX 전체가 아니라 등록된 명령만 그립니다. 지원하지 않는 명령은 글자로 남지 않고 칸이 통째로 비워집니다. 이 스킬은 `references/rules.md`의 허용 명령과 대체표를 근거로 수식을 옮기고 검수합니다.

## 할 수 있는 일

- **변환:** 교과서 문장이나 수식(사진·캡처 포함)을 Amplify용 백틱 LaTeX로 옮깁니다.
- **검수:** 직접 쓴 수식에 지원하지 않는 명령이 있는지 찾아 고칩니다.
- **질문:** 특정 명령이 Amplify에서 그려지는지 규칙 파일에 근거해 답합니다. 목록에 없으면 "확인되지 않았다"고 답합니다.

## 구성

```
SKILL.md              스킬 본체 (이름·설명·작업 절차)
instructions.md       지침 요약본 (스킬을 쓰지 않는 AI 도구에 붙여 넣는 용도)
references/rules.md   허용 명령, 대체표, 경로별 작성법
```

## 설치 방법 (개요)

스킬이 레포 루트에 있으므로 레포 주소만으로 설치합니다.

- **Gemini CLI:** `gemini skills install https://github.com/getbetterwithu/amplify-math`
- **Claude Code:** 이 레포를 `~/.claude/skills/amplify-math/`에 복제합니다.
  `git clone https://github.com/getbetterwithu/amplify-math ~/.claude/skills/amplify-math`
- **그 밖의 AI 도구:** `instructions.md`를 지침으로 붙여 넣고 `references/rules.md`를 첨부합니다.

> 설치 명령은 도구 버전에 따라 다를 수 있습니다. 실제로 확인된 설치 방법과 결과는 이 문서를 갱신해 기록합니다.
