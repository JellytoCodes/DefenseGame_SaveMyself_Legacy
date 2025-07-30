# 🛡️ SaveMyself
**Single-player Defence Survival Game** – Final project for 1st-year, Semester 1 (2025)

---

<br>

## Project Overview
> “플레이어가 직접 컨트롤하는 디펜스를 만들어보고 싶다”는 아이디어에서 시작된 **싱글 플레이어 생존 디펜스** 게임입니다. 각 스테이지마다  
> 구조물·함정을 배치하고, 제한된 자원으로 아이템을 구매해 몰려오는 적을 모두 처치하면 다음 스테이지로 진입합니다.

* **장르** : Defence / Survival  
* **플랫폼** : Windows (UE 5.4.4)  
* **개발 기간** : 2025-05-09 ~ 2025-06-02  

---

<br>

## Core Gameplay Features
| 카테고리 | 설명 |
|---------|------|
| **Inventory** | 무게 기반 인벤토리, 드래그 & 드롭 지원 |
| **Shop / Supply Depot** | 스테이지 전 아이템 구매, 실시간 잔액·무게 검증 |
| **Structures & Traps** | Overlap 이벤트로 발동, 내구도·쿨타임 시스템 |
| **Monster AI** | UAIPerception(Sight) + FSM로 타깃 추적·공격 |
| **Stage Flow** | 준비 → 전투 → 결과(Result UI) → 다음 스테이지 |
| **Save / Load** | UE `SaveGame` 클래스로 진행도 저장 |

---

<br>

## Technical Highlights
* **Subsystem-oriented Architecture** – Item, Save 등을 전용 Subsystem 으로 분리해 의존성 최소화  
* **Event / Delegate Bus** – UI ↔ Gameplay 간 실시간 상태 동기화  
* **Data-Driven Design** – 구조물·트랩·아이템을 `DataTable_JSON`에서 로드
* **Modular AI** – Perception + FSM 로 확장성 확보  
* **HUD Framework** – 스테이지·HP·타이머 등 즉각 반영

---

<br>

## Quick Start
### Prerequisites
* **Unreal Engine 5.4.4** (Binary or Source)  
* **Visual Studio 2022** (+ “Game development with C++” workload)

<br>

## Author & Acknowledgements
**JellytoCodes – Programmer**  
**Thanks To. 강상용 교수님**  

