# 🚀 Vibe Coding Playbook

 

실제 프로젝트에서 반복 활용하기 위한 개인 **Vibe Coding Workflow & Toolkit**.

 

단순히 AI에게 코드를 생성시키는 것이 아니라, 

**기획 → 설계 → 구현 → 테스트 → 배포 → 개선**까지 일관된 프로세스로 개발하는 것을 목표로 한다.

 

---

 

## 🔄 Workflow

 

**Idea → PRD → Design → Architecture → Plan → Build → Test → Review → Deploy → Iterate**

 

---

 

## 🧭 Vibe Coding Process

 

| Step | Process | What to do | Main Tools | Skills / Extensions |

|---|---|---|---|---|

| 01 | 💡 Idea | 문제·목표·사용자 정의 | Gemini | Ideation |

| 02 | 📋 PRD | 요구사항·기능·완료조건 정의 | Gemini | PRD |

| 03 | 🎨 Design | UI/UX 및 User Flow 설계 | Figma / v0 | Figma MCP |

| 04 | 🏗️ Architecture | 기술 Stack·DB·API 구조 설계 | Gemini / Claude Code | CLAUDE.md / Architecture |

| 05 | 📝 Plan | 개발 가능한 Task 단위로 분해 | Claude Code | Planning Skill |

| 06 | 💻 Build | Task 단위 기능 구현 | Claude Code | Skills / MCP |

| 07 | 🧪 Test | 기능·API·E2E 테스트 | Claude Code / Playwright | Testing Skill / Hooks |

| 08 | 🔍 Review | 코드 품질·보안·요구사항 충족 검토 | Claude Code | Code Review Skill / Subagents |

| 09 | 🚀 Deploy | Repository 관리 및 서비스 배포 | GitHub / Vercel / Azure | Deploy Skill / Hooks |

| 10 | 🔄 Iterate | Issue → 수정 → 테스트 → 재배포 | GitHub Issues / Claude Code | Agent Workflow |

 

---

 

## 🧠 Core Stack

 

### Gemini — Think & Define

 

아이디어를 구체화하고 개발 전 필요한 요구사항과 설계를 정리한다.

 

**Main Use**

 

- Idea

- Research

- PRD

- User Story

- Acceptance Criteria

- Architecture 초안

 

### Claude Code — Plan & Execute

 

PRD와 Architecture를 기반으로 실제 Repository에서 개발 작업을 수행한다.

 

**Main Use**

 

- Repository 분석

- Task Planning

- Coding

- Debugging

- Testing

- Refactoring

- Code Review

- Git Workflow

 

---

 

## 📚 Playbook

 

### 01. 💡 Idea

 

해결하려는 문제와 사용자를 정의하고 아이디어를 구체화한다.

 

**Tool:** Gemini

 

---

 

### 02. 📋 PRD

 

기능, Scope, User Story, Functional Requirements, Acceptance Criteria를 정의한다.

 

**Tool:** Gemini

 

👉 [PRD 작성 가이드](docs/PRD.md)

 

---

 

### 03. 🎨 Design

 

PRD를 기반으로 화면 구조와 User Flow를 설계한다.

 

**Tools:** Figma / v0

 

👉 [Design 가이드](docs/DESIGN.md)

 

---

 

### 04. 🏗️ Architecture

 

기술 Stack, Frontend, Backend, Database, API 및 서비스 구조를 정의한다.

 

**Tools:** Gemini / Claude Code

 

👉 [Architecture 가이드](docs/ARCHITECTURE.md)

 

---

 

### 05. 📝 Plan

 

PRD와 Architecture를 기반으로 전체 개발 범위를 작은 Task로 분해한다.

 

**Tool:** Claude Code

 

👉 [Task Planning 가이드](docs/TASKS.md)

 

---

 

### 06. 💻 Build

 

Task 단위로 기능을 구현하고 실행 결과를 확인한다.

 

**Tool:** Claude Code

 

---

 

### 07. 🧪 Test

 

Unit / API / E2E Test를 수행하고 Acceptance Criteria 충족 여부를 확인한다.

 

**Tools:** Claude Code / Playwright

 

👉 [Testing 가이드](docs/TESTING.md)

 

---

 

### 08. 🔍 Review

 

구현 결과를 PRD와 비교하고 코드 품질·보안·구조를 검토한다.

 

**Tool:** Claude Code

 

---

 

### 09. 🚀 Deploy

 

GitHub를 기준으로 Version을 관리하고 실제 환경에 배포한다.

 

**Tools:** GitHub / Vercel / Azure

 

👉 [Deployment 가이드](docs/DEPLOYMENT.md)

 

---

 

### 10. 🔄 Iterate

 

사용자 Feedback과 Issue를 다시 Task로 전환하여 개발 사이클을 반복한다.

 

**Tools:** GitHub Issues / Claude Code

 

---

 

## 🤖 Claude Code Extensions

 

Claude Code는 프로젝트가 복잡해질수록 아래 기능을 활용하여 개발 환경을 확장한다.

 

### CLAUDE.md

 

Claude Code가 프로젝트에서 항상 알아야 하는 **Context와 개발 원칙**을 정의한다.

 

**Examples**

 

- Tech Stack

- Project Structure

- Build / Test 명령어

- Coding Convention

- 개발 원칙

 

---

 

### Skills

 

반복적으로 사용하는 개발 절차를 재사용 가능한 Workflow로 만든다.

 

**Examples**

 

- Planning Skill

- Testing Skill

- Code Review Skill

- Refactoring Skill

- Deploy Skill

 

---

 

### MCP

 

Claude Code를 외부 시스템 및 데이터와 연결한다.

 

**Examples**

 

- GitHub

- Figma

- Database

- Documentation

- Browser

 

---

 

### Hooks

 

특정 이벤트 발생 시 정해진 작업을 자동으로 실행한다.

 

**Example**

 

```text

Code Change

    ↓

Formatter

    ↓

Lint

    ↓

Test

```

 

---

 

### Subagents

 

복잡한 작업을 별도의 전문 Agent에게 위임한다.

 

**Example**

 

```text

Planner

   ↓

Developer

   ↓

Tester

   ↓

Reviewer

```

 

---

 

### Plugins

 

Skills, Hooks, MCP 등의 구성을 패키징하여 프로젝트 간 재사용한다.

 

---

 

## 🛠 Resources

 

실제 사용하는 **Tool, Skill, MCP 및 관련 링크**를 관리한다.

 

👉 [Tools / Skills / MCP](resources/tools.md)

 

---

 

## 📄 Templates

 

새로운 프로젝트를 시작할 때 복사해서 사용하는 표준 Template.

 

- [PRD Template](templates/PRD-template.md)

- [Architecture Template](templates/architecture-template.md)

- [Task Template](templates/tasks-template.md)

 

---

 

## 💬 Prompt Library

 

반복적으로 사용하는 Vibe Coding Prompt를 관리한다.

 

👉 [Prompt Library](prompts/prompt-library.md)

 

---

 

## 🗂 Repository Structure

 

```text

vibe-coding-playbook/

│

├── README.md

│

├── docs/

│   ├── PRD.md

│   ├── DESIGN.md

│   ├── ARCHITECTURE.md

│   ├── TASKS.md

│   ├── TESTING.md

│   └── DEPLOYMENT.md

│

├── templates/

│   ├── PRD-template.md

│   ├── architecture-template.md

│   └── tasks-template.md

│

├── prompts/

│   └── prompt-library.md

│

└── resources/

    └── tools.md

```

 

---

 

## 🔁 Development Loop

 

실제 개발에서는 전체 애플리케이션을 한 번에 생성하지 않고 **작은 단위의 개발 Loop**를 반복한다.

 

```text

PRD

↓

Architecture

↓

Plan

↓

Task

↓

Build

↓

Test

↓

Review

↓

Commit

↓

Next Task

```

 

> **Build small. Test often. Commit frequently.**

 

---

 

## 🎯 Principle

 

**Gemini로 생각하고, Claude Code로 실행한다.**

 

> **Think → Specify → Plan → Build → Test → Review → Ship → Iterate**
