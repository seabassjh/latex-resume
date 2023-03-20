# 📋 Resume
---
[![résumé last release](https://img.shields.io/github/release-date/simbleau/resume?logo=github&label=Last%20Release)](https://github.com/simbleau/resume/releases)
[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/simbleau/resume/ci.yml?logo=github&label=CI)](https://github.com/simbleau/resume/actions/workflows/ci.yml)

# 🤖 Deployment
Deployment is automated by [GitHub Actions](https://github.com/simbleau/resume/actions).
- Pushes to `main` trigger a new release of the [latest résumé, cv, and cover letter](https://github.com/simbleau/resume/releases/tag/latest), available in several formats.
  | Artifact               | Link                                                                          | Mirror                                         |
  | ---------------------- | ----------------------------------------------------------------------------- | ---------------------------------------------- |
  | Résumé                 | <https://seabassjh.github.io/resume/resume.html>                               | <https://seabassjh.github.io/resume/>           |
  | Résumé, Embedded       | <https://seabassjh.github.io/resume/resume-embed.html>                         | <https://seabassjh.github.io/resume/embed.html> |
  | Résumé, Download       | <https://github.com/seabassjh/resume/releases/download/latest/resume.pdf>      |                                                |
  | CV                     | <https://seabassjh.github.io/resume/cv.html>                                   |                                                |
  | CV, Embedded           | <https://seabassjh.github.io/resume/cv-embed.html>                             |                                                |
  | CV, Download           | <https://github.com/seabassjh/resume/releases/download/latest/cv.pdf>          |                                                |
  | Cover letter           | <https://seabassjh.github.io/resume/coverletter.html>                          |                                                |
  | Cover letter, Embedded | <https://seabassjh.github.io/resume/coverletter-embed.html>                    |                                                |
  | Cover letter, Download | <https://github.com/seabassjh/resume/releases/download/latest/coverletter.pdf> |                                                |
- Manually pushed [releases](https://github.com/simbleau/resume/releases) also trigger workflows to upload artifacts.

# 🔧 Building
## Dependencies
- [TeXLive, full](https://www.tug.org/texlive/)
- [Make](https://www.gnu.org/software/make/)
- [j2cli](https://github.com/kolypto/j2cli)
## Commands
- **Build the résumé**:
  ```bash
  make resume
  ```
- **Build the cirriculum vitae**:
  ```bash
  make cv
  ```
- **Build the cover letter**:
  ```bash
  make coverletter
  ```
- **Build all**:
  ```bash
  make all
  ```
- **Purge all**:
  ```bash
  make clean
  ```
- **Open PDFs**:
  ```bash
  make open
  ```
