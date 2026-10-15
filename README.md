1. What to select on GitHub's "Create a new repository" page:
Repository description: Paste the short description:
Professional QGIS print layout studio with 50 clean cartographic templates across diverse layout architectures, automated layer binding, preflight QA, and publication export. Developed by Ariesplus Geospatial Solution.

Add README toggle: Leave it OFF (as shown in your screenshot).
Why: Because your local folder already contains this comprehensive README.md. Leaving it off allows you to push your existing project cleanly without Git merge conflicts.
2. Complete Content of Your Updated README.md
markdown
# MapTemplate Studio — QGIS Plugin
> **A high-resolution, cartography-ready QGIS print layout template studio with 50 pure white templates across 14 layout architectures.**  
> *Developed by **Ariesplus Geospatial Solution***
[![QGIS Compatibility](https://img.shields.io/badge/QGIS-3.28%2B%20%7C%204.x-589632.svg?logo=qgis&logoColor=white)](https://qgis.org)
[![Qt 5 & 6](https://img.shields.io/badge/Qt-5%20%26%206%20Compatible-41cd52.svg?logo=qt&logoColor=white)](https://qt.io)
[![License: GPL-2.0-or-later](https://img.shields.io/badge/License-GPL--2.0--or--later-blue.svg)](LICENSE)
[![Templates: CC-BY-4.0](https://img.shields.io/badge/Templates-CC--BY--4.0-orange.svg)](docs/LICENSE_REGISTER.csv)
[![Tests: 27 Passed](https://img.shields.io/badge/Tests-27%20Passed-success.svg)](tests/)
[![Author](https://img.shields.io/badge/Author-Ariesplus%20Geospatial%20Solution-0f172a.svg)](mailto:ariesplusgeo@gmail.com)
---
## 📌 Overview
**MapTemplate Studio** is a production-grade QGIS plugin developed by **Ariesplus Geospatial Solution**. It empowers GIS professionals, cartographers, urban planners, surveyors, researchers, and remote sensing analysts with an interactive, searchable gallery of **50 original print layout templates**.
All templates are designed with a **clean white cartographic theme** (`#ffffff` canvas, crisp dark slate `#334155` / `#0f172a` neatlines, and high-contrast charcoal typography) across **14 distinct layout architectures**—from formal cadastral survey sheets and executive KPI dashboards to twin-viewport multi-temporal comparisons and presentation slides.
---
## 🎨 Consistent with QGIS Software UI Theme
MapTemplate Studio is built to look, feel, and behave like an integrated component of QGIS Desktop:
- **Adaptive Light & Dark Modes**: Dynamically detects the QGIS desktop palette (*Default Light* or *Night Mapping Dark*) and adjusts backgrounds, cards, text, and inputs accordingly.
- **Native QGIS Widgets**: Utilizes `QgsCollapsibleGroupBox`, `QgsFilterLineEdit` with live search and clear buttons, `QgsMapLayerComboBox` with native layer geometry icons, and `QgsFileWidget`.
- **QGIS Cartographic Brand Accents**: Clean QGIS green accenting (`#589632`), standard 6–8px padding, and responsive status pills.
- **Flexible Docking**: Operates as a native `QDockWidget` that docks into either side of QGIS or floats freely.
---
## 📐 14 Distinct Layout Architectures
Every template is tailored to a specific communicative purpose, utilizing one of 14 architectural layouts:
| Layout Architecture | Description | Target Use Cases |
| :--- | :--- | :--- |
| **Standard Hero Landscape** | Landscape map with dedicated top header block and bottom marginalia bar | Reference, administrative, environmental risk (`GEN-01`, `RS-01`, `ENV-01`) |
| **Corner Floating Full-Bleed** | Full-bleed map with floating white title card, legend card, and scale/north block | Continuous surfaces, NDVI, imagery indices (`RS-03`, `ENV-04`, `TER-05`) |
| **Left Rail Column** | Large map viewport on right, dedicated left column with regional locator map & legend | Regional growth, urban corridor redevelopment (`PLN-04`, `PLN-05`, `URB-01`) |
| **Right Rail Column** | Main map on left, dedicated right column with locator map, legend, and metadata | District profiles, emergency situation reports (`GEN-06`, `PLN-01`, `EMR-01`) |
| **Bottom Band Master** | Expansive A3/A2 master map on top with a 4-column marginalia panel below | Comprehensive master zoning, topographic contours (`PLN-02`, `TER-02`, `URB-03`) |
| **Minimal Portrait Figure** | Clean portrait figure with formal academic caption and figure numbering below | Theses, dissertations, peer-reviewed journals (`GEN-02`, `EDU-01`) |
| **Executive Report Portrait** | A4 portrait map with a 3-column bottom control panel (legend, scale, projection, source) | Municipal profiles, thermal surveys, social vulnerability (`GEN-03`, `RS-04`, `ENV-03`, `SOC-04`) |
| **Right Rail Portrait** | Portrait map with a dedicated right sidebar column for legend, north arrow, and stats | Multi-criteria suitability, population choropleths (`PLN-03`, `SOC-01`, `URB-02`) |
| **Cadastral Survey Plan** | Double neatlines (0.6mm outer, 0.25mm inner) with formal **Surveyor's Certificate & Seal Box** | Cadastral parcels, geodetic control sheets (`SUR-01`, `SUR-02`) |
| **Split Compare Horizontal** | Twin side-by-side synchronized viewports with baseline (T1) and observed (T2) headers | Before-and-after change, multi-sensor radar vs optical (`ATL-02`, `RS-02`, `RS-05`, `ENV-02`) |
| **Executive Dashboard** | Main map with territorial context map and **metric KPI indicator cards** with bold numerals | Asset governance, executive briefings, emergency sitreps (`GEN-05`, `EMR-04`) |
| **Atlas Series Sheet** | Dynamic map series sheet with `[% @atlas_pagename %]` and series locator index | Ward index, district atlas series (`ATL-01`, `ATL-03`) |
| **Widescreen 16:9 Slide** | 16:9 landscape format optimized for digital slide decks with right briefing card | Executive PowerPoint/Keynote briefings (`DIG-01`) |
| **Compact Briefing Card** | A5 landscape compact card with embedded legend and scale | Social media, web summaries, rapid briefs (`DIG-02`) |
---
## 🗂️ Complete 50-Template Catalog
The 50 templates are categorized across **12 thematic families**:
```text
├── General & Reference (7)        │ GEN-01 to GEN-07
├── Urban Planning & Zoning (5)    │ PLN-01 to PLN-05
├── Remote Sensing & Imagery (6)   │ RS-01 to RS-06
├── Environment & Hazard (5)       │ ENV-01 to ENV-05
├── Terrain & Geomorphology (5)    │ TER-01 to TER-05
├── Social & Demographics (4)      │ SOC-01 to SOC-04
├── Transport & Mobility (4)       │ URB-01 to URB-04
├── Humanitarian & Emergency (4)   │ EMR-01 to EMR-04
├── Cadastral & Surveying (3)      │ SUR-01 to SUR-03
├── Atlas & Multi-Map (3)          │ ATL-01 to ATL-03
├── Academic & Publishing (2)      │ EDU-01 to EDU-02
└── Digital & Presentation (2)     │ DIG-01 to DIG-02
🚀 Key Features
1. Interactive Template Gallery Dock
Real-time instant search by template name, keywords, author, or map roles.
Filter by 12 Thematic Families, 6 Page Archetypes, and Paper Sizes (A4, A3, A2, A5, 16:9).
Quick-access Favorites (Star) and Recently Used sections.
High-resolution thumbnails showing exact white cartographic layout geometry.
2. Four-Stage Guided Creation Wizard
Step 1: Template & Style: Select template, view metadata, and choose your preferred paper size and orientation.
Step 2: Map Content & Roles: Seamlessly bind active QGIS project layers to layout viewports (main_map, locator_map, before_map, after_map) with automated extent fitting (Canvas, Layer, or Fixed Scale) and margin padding.
Step 3: Cartography & Marginalia: Configure Title, Subtitle, Sources, Surveyor/Author attribution, Date, CRS, dynamic scale bars, north arrows, and logos.
Step 4: Preflight & Output: Inspect real-time QA validation, view the readiness score, and generate the editable QgsPrintLayout.
3. Preflight Quality Assurance Engine
Automatic QA inspection prevents bad exports before they happen:

Detects unmapped required map roles, empty extents, or broken linkages.
Flags missing title, scale bar, north arrow, or projection metadata.
Calculates an automated Readiness Score (0–100%) with clear Pass, Warning, and Blocker remediation instructions.
4. Production Multi-Format Exporter
Export directly with production presets or open the native composer:

Print PDF (300 DPI & 600 DPI) with vector geometry preservation.
Geospatial PDF with embedded georeferencing and layer trees.
Digital 4K & Full HD PNG (3840×2160 / 1920×1080).
Scalable Vector Graphics (SVG) and GeoTIFF / High-Res TIFF.
Real-time raster memory safety estimator to prevent out-of-memory crashes on large plotters.
5. Custom Template Importer (.qpt)
Safely inspects and imports third-party or organizational .qpt templates into your local library with path-traversal sandboxing.
6. 100% Offline-First
Zero external cloud dependencies. All 50 templates, XML schemas, and preview assets are bundled locally.
💻 Installation
Method 1: Install from ZIP in QGIS (Recommended)
Download the latest release: 

maptemplate_studio.zip
.
In QGIS, navigate to Plugins → Manage and Install Plugins....
Select Install from ZIP on the left menu.
Browse to the downloaded maptemplate_studio.zip file and click Install Plugin.
MapTemplate Studio will appear in your panels and toolbar!
Method 2: Manual Directory Installation
Clone or copy the repository directly into your QGIS profile's plugin directory:

Windows:
powershell
%APPDATA%\QGIS\QGIS4\profiles\default\python\plugins\maptemplate_studio
Linux:
bash
~/.local/share/QGIS/QGIS3/profiles/default/python/plugins/maptemplate_studio
macOS:
bash
~/Library/Application Support/QGIS/QGIS3/profiles/default/python/plugins/maptemplate_studio
🧪 Testing & Verification
The plugin includes a full unit test suite ensuring 100% reliability across headless environments:

powershell
& "C:\Program Files\QGIS 4.2.1\bin\python-qgis.bat" -m unittest discover tests -v
Results: 27 tests passed (0 errors, 0 failures), verifying:

Schema validation for all 50 template manifests
Search, filter, favorite, and recent caching logic
Automated bounding box aspect-ratio calculations and margin expansion
Non-destructive QgsPrintLayout generation and item role binding
Headless PDF and PNG generation
Dark/light mode theme awareness
📁 Repository Structure
text
MapTemplate Studio/
├── metadata.txt               # QGIS official plugin metadata (v1.0.0)
├── LICENSE                    # GNU General Public License v2.0+
├── README.md                  # Comprehensive plugin documentation
├── __init__.py                # QGIS classFactory initialization
├── main_plugin.py             # Plugin lifecycle, menu actions, toolbars
├── icon.png                   # High-res 64x64 QGIS-styled plugin icon
│
├── core/                      # Headless core business logic
│   ├── catalog_service.py     # Discovers, indexes, and searches templates
│   ├── manifest_validator.py  # JSON Schema and integrity validation
│   ├── template_importer.py   # Sandboxed .qpt parser and custom template manager
│   ├── layout_factory.py      # Non-destructive QgsPrintLayout constructor
│   ├── role_binder.py         # Dynamic layer, legend, scale, and text binding
│   ├── extent_scale.py        # Frame-aspect extent fitting and scale calculation
│   ├── preflight.py           # Cartographic QA preflight engine
│   ├── exporter.py            # Multi-format production exporter
│   ├── asset_resolver.py      # Path and asset resolution
│   └── settings_service.py    # Persistent user preferences (QgsSettings + JSON)
│
├── ui/                        # Native QGIS Theme UI Components
│   ├── theme.py               # Palette awareness, light/dark mode QSS, theme icons
│   ├── template_model.py      # TemplateCardWidget with thumbnails & pills
│   ├── gallery_dock.py        # Dockable gallery studio with category sidebar
│   ├── wizard_dialog.py       # 4-stage guided creation wizard
│   ├── preflight_dialog.py    # Cartographic QA preflight inspector
│   ├── export_dialog.py       # High-resolution production export dialog
│   └── import_template_dialog.py # Custom .qpt importer dialog
│
├── templates/                 # 50 Production-Grade Pure White Templates (GEN-01 ... DIG-02)
├── schema/                    # Manifest JSON Schema definition
├── styles/                    # Color tokens and cartographic standards
├── tests/                     # 27 automated unit tests
└── docs/                      # User guide, template authoring guide, license register
