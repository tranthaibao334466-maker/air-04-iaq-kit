# CLAUDE.md

## Goal
Design a STEM learning kit for indoor air quality (lower and upper secondary students), using Design Thinking. The flagship study is bedroom air quality.
- `project-idea.md` is the north star. Read it before every task and run its "Alignment check".
- University course project: Microprocessor major assignment (Bài tập lớn Vi xử lý), class ETTN-K69, a team of 4. The team's weekly record is `nhat-ky-ky-thuat.docx`.
- Current phase: Empathize/Define. The original brief `requirements.docx` was removed on purpose. Do not ask for it and do not cite it as a current source.

## Directory layout
```
iaq/
├─ CLAUDE.md
├─ project-idea.md          # READ-ONLY for Claude: only the user edits it
├─ nhat-ky-ky-thuat.docx    # team engineering log (Word), see "Engineering log"
├─ decisions.md             # phase decisions, written only on the user's explicit confirmation
└─ notes/
   └─ week-NN/              # intermediate .md syntheses, e.g. notes/week-06/competitor-analysis.md
```
- Create other folders only when needed, and say so when you do.
- Week numbers: Week 1 = 05/10/2026–11/10/2026, and each week runs Monday to Sunday. Use two digits (`week-06`).

## Engineering log (`nhat-ky-ky-thuat.docx`)
- Workflow:
  1. Synthesise findings into `.md` files in `notes/week-NN/`.
  2. Add the new content to `nhat-ky-ky-thuat.docx`, **updating the original file directly**. No approval is needed for this file.
- Follow the existing template exactly:
  - Each week has: `Tuần N: dd/mm/yyyy → dd/mm/yyyy`, a week theme line, then 1. Mục tiêu đầu tuần, 2. Bảng phân công công việc, 3. Nội dung chi tiết (3.x set by the phase), 4. Khó khăn và kết quả cuối tuần (4.1 Khó khăn…, 4.2 Kết quả chốt cuối tuần, 4.3 Kế hoạch tuần sau).
  - Use the existing Word styles: Heading1/2/3, ListParagraph, the table layouts and the caption under each table and figure.
  - End every 3.x subsection with a line `Nguồn: [tên tài liệu / tác giả / đường dẫn / năm]`.
- For a week not yet in the file, copy the week skeleton above.
- Content must follow `project-idea.md` (a learning kit with bedroom air quality as the flagship study). Where the log still frames the project as a plain bedroom meter (AIR-04), rewrite that content to match `project-idea.md`.
- Never change team members' names, student IDs, the class or the supervisor, and never invent task assignments. Leave `[Tên thành viên]` if unknown.
- Edit the .docx with the docx skill. If a tool it needs is missing, stop and ask. Never install anything.

## Solutions vs. needs (most important rule)
- Do not lock in solutions before the user confirms the SPECs. Specific hardware, platforms or tools (for example ESP32, SCD41, Scratch, Arduino) may be mentioned only as **[Tham khảo]**, each with at least one alternative.
- Write no firmware or device code until the user has confirmed the SPECs in `decisions.md`.
- Keep the bedroom air quality study central. Every other activity must serve it or lead toward it.

## Decisions (`decisions.md`)
- Record a decision only when the user says explicitly that it is decided ("đã chốt"). Record the date, the phase, the decision and its basis (with sources).
- The file is a draft and is refined over time. Never mark something as decided on your own.

## Language and style
- Chat: Vietnamese, detailed, with examples.
- Project documents (.md and log content): Vietnamese Markdown. File names: English kebab-case (`teacher-interview-01.md`).
- This file and `project-idea.md` are in English.

## Honesty about sources
- Every number (price, spec, statistic) needs a source link.
- Label each claim: **[Nguồn]** (found, with link), **[Kiến thức chung]**, **[Suy luận]**, **[Giả định]**.
- Look up facts that change before using them: prices, products, datasheets, Ministry of Education documents. Prefer academic, official and datasheet sources.
- Never invent citations, documents or document numbers. If something cannot be verified, say so.
- Illustrative numbers are allowed only when marked: "Số liệu giả định – thay bằng dữ liệu thật".
- Web search is allowed. Never put personal data (names, emails, student IDs) in queries.

## Data and privacy
- Only de-identified data belongs in this folder. Never open, read or ask for non-de-identified data (names of students or parents, contact details).
- Never present readings or findings as a medical diagnosis.

## Environment
- Windows 11. Shells: PowerShell (primary) and Git Bash. Python is not installed. Analysis tools are not chosen yet: propose one and ask before using any.
- Allowed: reading and listing files; building or compiling code and running scripts.
- Not allowed: installing software or libraries; flashing or uploading firmware to devices.
- No git: do not run git commands.

## Working with files
- New files: create them freely and tell the user the path.
- Existing files: ask before editing. Exceptions: `nhat-ky-ky-thuat.docx` (update directly, see above) and files in `notes/` that you created in the same task.
- `project-idea.md`: never edit it. Propose changes in chat instead.
- If a request is unclear or could go several ways, ask before acting, and offer the options.

## Reports
End every document you create with these three sections:
1. **Nguồn tham khảo**: the links used.
2. **Giả định cần kiểm chứng**: what is not yet verified.
3. **Đối chiếu project-idea.md**: which part of the idea, the flagship study and the constraints this serves.

## Hard rules
- Never delete files, including files you created.
- Never use paid services or paid APIs.
- Never send content outside: no email, posting or sharing files.
- Never read non-de-identified personal data.
- Never edit `project-idea.md`.
- Never install software, flash devices or run git.
