<!-- VM Wizard generated — do not edit by hand. Re-run Install Tools or Restore Tools. -->
# OS and tools (this project)

**Generated:** 2026-11-09T09:05:54Z · **Project root:** `D:/Temp/-----/smart-money-concepts`

## Host

| Item | Value |
|------|--------|
| OS family | **Windows** (`osSubtype`: Native) |
| OS version | Microsoft Windows NT 10.0.26300.0 |
| Shell | PowerShell — do **not** use bash, apt, or Linux-only commands on Windows Native |
| CPU arch | x64 |

## Project tools (VM `.tools/` — use these only)

Do **not** use `python`, `python3`, `node`, or `npm` from global PATH unless this file explicitly allows it.

### Python

Use the **venv** interpreter for running code and `pip install`. Do not use global Python.

| | Path |
|---|------|
| **venv (preferred)** | `.tools/.python/venv/Scripts/python.exe` |
| venv absolute | `D:/Temp/-----/smart-money-concepts/.tools/.python/venv/Scripts/python.exe` |
| Embed base | `.tools/.python/python.exe` |
| Embed absolute | `D:/Temp/-----/smart-money-concepts/.tools/.python/python.exe` |
| Version | 3.10.11 (embed-3.10-win-x64 + pip/venv) |

Example: `.\.tools\.python\venv\Scripts\python.exe -m pip install <package>`

### Node.js

Use project-local **`npm.cmd` / `npx.cmd`** (bundled with portable Node). Do not use global `npm` from PATH.

| | Path |
|---|------|
| node | `.tools/.nodejs/node.exe` |
| node absolute | `D:/Temp/-----/smart-money-concepts/.tools/.nodejs/node.exe` |
| **npm (preferred)** | `.tools/.nodejs/npm.cmd` |
| npm absolute | `D:/Temp/-----/smart-money-concepts/.tools/.nodejs/npm.cmd` |
| npx | `.tools/.nodejs/npx.cmd` |
| npx absolute | `D:/Temp/-----/smart-money-concepts/.tools/.nodejs/npx.cmd` |
| Version | 22.16.0 (official win-x64 zip includes npm) |

**Where to run npm:**

- Find an existing `package.json` (often under `Web/`, `frontend/`, or another app folder) and run npm **there**.
- Do **not** create a new root `package.json` only to try a package, and do **not** invent a project just for a smoke test.
- If no app `package.json` exists and the task needs one, ask the user which folder should own Node dependencies.

Example (from repo root, targeting an app folder): `.\.tools\.nodejs\npm.cmd --prefix Web install <package>`
Example: `.\.tools\.nodejs\node.exe --version`

## Allowed and forbidden

- **Use:** commands in this file, .NET SDK, VM `.tools/` runtimes.
- **Do not use:** LibreOffice, undocumented CLI, Linux paths (`/tmp`, `rm -rf`), or global Python/Node when project tools are installed.
- **Agents:** obey the OS family in the Host table — do not assume Linux on Windows Native.
