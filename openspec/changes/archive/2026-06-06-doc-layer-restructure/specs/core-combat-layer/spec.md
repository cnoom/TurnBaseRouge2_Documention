## ADDED Requirements

### Requirement: Core combat module files move to layered directories

The files under `01_核心战斗/` SHALL be moved into four layer subdirectories per the table in design.md.

#### Scenario: All files placed in correct layer directory
- **WHEN** the restructuring is applied
- **THEN** each file under `01_核心战斗/` exists in exactly one of `01_规范/`, `02_机制/`, `03_数据/`, `04_校验/`
- **THEN** no `.md` files remain directly under `01_核心战斗/` (except `敌人配置数据/` subdirectory)

#### Scenario: 敌人幕间强度.md split into three files
- **WHEN** the restructuring is applied
- **THEN** the file `01_核心战斗/敌人幕间强度.md` no longer exists
- **THEN** the file `01_核心战斗/03_数据/敌人幕间/幕间增长原则.md` exists containing design principles, growth curve multipliers, enemy pool allocation, and player growth comparison
- **THEN** the file `01_核心战斗/03_数据/敌人幕间/普通敌人增长曲线.md` exists containing all 5 normal enemy per-act detailed action tables
- **THEN** the file `01_核心战斗/03_数据/敌人幕间/精英与Boss增长曲线.md` exists containing all 2 elite and 4 boss per-act detailed action tables
- **THEN** the original `敌人幕间强度.md` is moved to `归档/`

### Requirement: Relic data files grouped into subdirectory

The files `普通遗物.md` and `稀有遗物.md` SHALL be moved into `01_核心战斗/03_数据/遗物/`.

#### Scenario: Relic files in correct location
- **WHEN** the restructuring is applied
- **THEN** `普通遗物.md` exists at `01_核心战斗/03_数据/遗物/普通遗物.md`
- **THEN** `稀有遗物.md` exists at `01_核心战斗/03_数据/遗物/稀有遗物.md`
- **THEN** the original locations no longer contain these files
