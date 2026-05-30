# ATS-Safe Formatting Checklist

Applicant Tracking Systems parse resumes as plain text before a human sees them. Anything that confuses the parser can drop a qualified candidate. Apply these to the CV .docx.

## Layout
- **Single column, linear top-to-bottom.** Multi-column layouts get read out of order or scrambled.
- **No tables** for content. Many parsers read tables cell-by-cell or skip them. (A borderless single-cell wrapper is risky too — avoid.)
- **No text boxes, no SmartArt, no shapes.** Parsers often ignore them entirely — text inside vanishes.
- **No critical info in headers/footers.** Some parsers never read them. Put name, phone, email in the body.
- **No images, logos, icons, or charts.** They carry no parseable text and can break extraction.

## Typography
- Standard fonts only: Calibri, Arial, Helvetica, Garamond, Georgia, Times New Roman.
- Body 10-12 pt; name 16-22 pt. Don't go below 10 pt.
- Use real **bold**/italic, not letter-spacing tricks or all-caps as emphasis everywhere.

## Structure & headings
- Use conventional section titles the parser recognizes: **Summary / Professional Summary, Skills / Core Competencies, Experience / Professional Experience, Education, Publications, Certifications, Projects.** Avoid cute headings ("Where I've Made Dents").
- Reverse-chronological order within Experience.
- Each role: Title — Organization — Location — Dates (consistent format, e.g., `Jan 2023 – Present` everywhere; don't mix `2023` and `01/23`).
- Bullets as genuine list items (real bullet character / Word list), not manual dashes with odd spacing.

## Content for ATS matching
- Mirror the **exact keyword strings** from the target description where truthful (e.g., if the JD says "time-series forecasting", use that phrase, not just "predictive modeling").
- Spell out **and** abbreviate key terms once: "natural language processing (NLP)" — parsers and recruiters search both.
- Put the most important skills/keywords **high** (summary + skills section), since some parsers weight position.
- Keep a dedicated **Skills** section with scannable, comma- or pipe-separated terms grouped by type (Languages, ML/Stats, Tools, Domains).

## Honesty guardrail
Only include skills/keywords the candidate genuinely has. If the target demands a keyword the candidate lacks, list it under "gaps to close" in the chat summary — never silently insert a false claim. ATS gets you screened in; a human and an interview get you hired, and fabrications surface fast.

## File
- Deliver as `.docx` (most ATS-friendly alongside plain text). Avoid PDF only if the posting specifically warns against it; otherwise .docx is the safe default.
- Filename: `CV_<Name>_<Target>.docx` — clean, no spaces-to-underscores chaos, no version cruft like `final_v3_REAL`.
