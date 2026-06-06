## ADDED Requirements

### Requirement: README.md navigation links updated

All file path references in `README.md` quick navigation table SHALL be updated to match the new layered directory paths.

#### Scenario: All navigation links point to correct new paths
- **WHEN** the restructuring is applied
- **THEN** every URL in the README.md navigation table that references a moved file points to the correct new layered path
- **THEN** the README.md also reflects the new directory structure for 03_进度与成长 and 05_体验与表现 (from 🔲 to showing the layer structure)

### Requirement: Data dictionary "influenced documents" column updated

The file `00_总纲/数据字典.md` SHALL have all file path references in the "影响文档" column updated to match the new layered paths.

#### Scenario: All data dictionary path references correct
- **WHEN** the restructuring is applied
- **THEN** every path-like reference in 数据字典.md's "影响文档" column points to a valid file in the new layered structure

### Requirement: Documentation architecture guide updated

The file `文档架构说明.md` SHALL have its directory structure diagram updated to reflect the new layered structure.

#### Scenario: Architecture guide shows layered structure
- **WHEN** the restructuring is applied
- **THEN** the directory structure diagram in `文档架构说明.md` shows the four layer subdirectories under each module
