# amplify-math

Amplify Classroom(Desmos)의 메모·수식 답변·CL에 들어갈 수학 수식을 작성·검수·변환하는 스킬입니다.

Amplify의 수식은 표준 LaTeX 전체가 아니라 등록된 명령만 그립니다. 지원하지 않는 명령은 글자로 남지 않고 칸이 통째로 비워집니다. 이 스킬은 `references/rules.md`의 허용 명령과 대체표를 근거로 수식을 옮기고 검수합니다.

## 할 수 있는 일

- **변환:** 교과서 문장이나 수식(사진·캡처 포함)을 Amplify용 백틱 LaTeX로 옮깁니다.
- **검수:** 직접 쓴 수식에 지원하지 않는 명령이 있는지 찾아 고칩니다.
- **질문:** 특정 명령이 Amplify에서 그려지는지 규칙 파일에 근거해 답합니다. 목록에 없으면 "확인되지 않았다"고 답합니다.

## 구성

```
skills/amplify-math/SKILL.md              스킬 본체 (이름·설명·작업 절차)
skills/amplify-math/instructions.md       지침 요약본 (스킬을 쓰지 않는 AI 도구에 붙여 넣는 용도)
skills/amplify-math/references/rules.md   허용 명령, 대체표, 경로별 작성법
```

## 설치 방법 (개요)

레포 주소만으로 설치합니다.

- **Claude Code** (확인됨):
  ```
  claude plugin marketplace add getbetterwithu/amplify-math
  claude plugin install amplify-math@amplify-math
  ```
  설치 후 `claude plugin list`에서 `amplify-math@amplify-math`가 enabled로 보이면 됩니다. 다음 세션부터 적용됩니다.
- **Antigravity** (`agy`):
  ```
  agy plugin install https://github.com/getbetterwithu/amplify-math
  agy plugin list
  ```
  설치 결과에 `skills : 1 processed`가 보이면 됩니다. 이전에 설치해 빈 플러그인이 남아 있다면 `agy plugin uninstall amplify-math` 후 다시 설치합니다.
- **그 밖의 AI 도구** (ChatGPT 등): `skills/amplify-math/instructions.md`를 지침으로 붙여 넣고 `skills/amplify-math/references/rules.md`를 첨부합니다.
