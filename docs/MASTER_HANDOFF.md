# MASTER HANDOFF: Vibe Coding AI Puppet System
## For: Gemini CLI (Full Autonomous Authority)

**Status:** Ready for handoff  
**User:** Dawn (JKEATS)  
**Hardware:** HP ProBook 6560b | Windows 10 Home | 8GB RAM | i3-2310M @ 2.10GHz  
**Storage:** C:\ (512GB internal) | E:\ (931GB external Seagate)  
**Project Root:** `/home/ubuntu/vibe_coding_puppet` (Manus sandbox) + `C:\projects\vibe_coding_puppet` (Windows)  
**Authority Level:** FULL YOLO MODE - Complete autonomy to execute, modify, debug, and iterate

---

## MISSION STATEMENT

Build a **personal creative AI studio** that generates and manages cohesive, high-quality web assets:
- **HTML/CSS snippets** — Reusable, styled code blocks
- **JavaScript functions** — Interactive components and utilities
- **Full website templates** — Production-ready sites with unified aesthetics
- **Design system** — Consistent colors, typography, spacing, and patterns

All assets are stored on the external SSD (E:\) with full metadata indexing, searchability, and organization. The system is designed to be a "puppet" that takes commands and produces polished, on-brand creative work.

---

## HARDWARE CONTEXT (Critical for Optimization)

### System Specifications
| Component | Details |
|-----------|---------|
| **Computer** | HP ProBook 6560b |
| **OS** | Windows 10 Home (Build 19045) |
| **CPU** | Intel Core i3-2310M @ 2.10GHz |
| **RAM** | 8 GB total (currently ~1.2GB available) |
| **Network** | Wi-Fi: Intel Centrino Advanced-N 6205 |
| **Timezone** | Eastern Time (UTC-05:00) |

### Storage Configuration
| Drive | Type | Capacity | Mount | Purpose |
|-------|------|----------|-------|---------|
| **Internal** | SSD 512GB | ~477 GB | C:\ | OS, apps, active development |
| **External** | Seagate One Touch SSD | ~931 GB | E:\ | Asset library, backups, archives |

### Critical Constraints
- **RAM is tight:** Only 8GB total, ~1.2GB currently available
- **CPU is older:** i3-2310M is from 2012; avoid heavy computational tasks
- **Disk I/O:** SSDs are fast, but network/cloud operations may be slow
- **Development environment:** Must be lightweight and efficient

---

## ARCHITECTURE OVERVIEW

### Layer 1: Frontend (React 19 + Tailwind 4)
- **Location:** `C:\projects\vibe_coding_puppet` (Windows) | `/home/ubuntu/vibe_coding_puppet` (Manus)
- **Tech Stack:** React 19, Tailwind CSS 4, shadcn/ui, Wouter (routing)
- **Purpose:** Dashboard to browse, search, filter, and manage assets
- **Key Features:**
  - Asset library browser (grid/list view)
  - Code editor with syntax highlighting
  - Design system manager
  - Search and filter by category, style, date, tags
  - Export functionality (ZIP, individual files)

### Layer 2: Asset Library (E:\ External SSD)
- **Root:** `E:\vibe_coding_puppet\`
- **Structure:**
  ```
  E:\vibe_coding_puppet\
  ├── generated_websites/        # Full website templates
  ├── component_library/         # HTML/CSS/JS snippets
  ├── design_assets/
  │   ├── images/
  │   ├── icons/
  │   ├── fonts/
  │   └── color_palettes/
  ├── templates/                 # Boilerplate structures
  ├── backups/                   # Weekly project backups
  ├── asset_index.json           # Master metadata file
  ├── design_system.json         # Color, typography, spacing definitions
  └── README.md                  # Asset library documentation
  ```

... (rest of MASTER_HANDOFF content)
