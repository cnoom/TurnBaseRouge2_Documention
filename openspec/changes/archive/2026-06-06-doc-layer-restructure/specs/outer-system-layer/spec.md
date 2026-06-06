## ADDED Requirements

### Requirement: Outer system module files move to layered directories

The files under `02_局外系统/` SHALL be moved into layer subdirectories per the design.

#### Scenario: All files placed in correct layer directory
- **WHEN** the restructuring is applied
- **THEN** each file under `02_局外系统/` exists in exactly one of `01_规范/`, `02_机制/`, `03_数据/`
- **THEN** no `.md` files remain directly under `02_局外系统/`

#### Scenario: New spec file 关卡设计规范.md created
- **WHEN** the restructuring is applied
- **THEN** the file `02_局外系统/01_规范/关卡设计规范.md` exists containing design principles for level structure, difficulty gradient, and option types

### Requirement: 事件系统.md split into four files

The file `02_局外系统/事件系统.md` (431 lines) SHALL be split into four files by content type.

#### Scenario: 事件设计规范.md created with spec content
- **WHEN** the restructuring is applied
- **THEN** the file `02_局外系统/01_规范/事件设计规范.md` exists containing: design principles, event type taxonomy (6 types), modifiable attribute dimensions with gold-value anchors, and event pool structure definition

#### Scenario: 事件流程机制.md created with mechanism content
- **WHEN** the restructuring is applied
- **THEN** the file `02_局外系统/02_机制/事件流程机制.md` exists containing: trigger flow, high-risk enhancement rules (3 types), continuous chain event rules, and cross-system dependencies

#### Scenario: 正面事件池.md and 混合事件池.md created with data content
- **WHEN** the restructuring is applied
- **THEN** the file `02_局外系统/03_数据/正面事件池.md` exists containing all 10 positive event data tables (each with flavor text, options, effects, type tags)
- **THEN** the file `02_局外系统/03_数据/混合事件池.md` exists containing all 10 mixed event + 2 chain event data tables
- **THEN** the original `事件系统.md` is moved to `归档/`

### Requirement: 商店系统/奖励系统暂留原内容不拆分

The files `商店系统.md` and `奖励系统.md` SHALL be moved to `02_机制/` without content splitting.

#### Scenario: Store and reward files moved as-is
- **WHEN** the restructuring is applied
- **THEN** `商店系统.md` exists at `02_局外系统/02_机制/商店系统.md`
- **THEN** `奖励系统.md` exists at `02_局外系统/02_机制/奖励系统.md`
- **THEN** their content remains unchanged
