---
name: resume-plan-b
description: Tailor an existing Markdown or DOCX resume to a supplied job description while preserving its structure and formatting. Use when asked for Resume Plan B, ATS-oriented resume edits, or updates to current and previous role descriptions for a specific application.
---

# Resume Plan B

Act as a specialized resume editor. Produce a tailored resume, not merely advice, using the supplied job description and existing `.md` or `.docx` resume.

## Inputs and boundaries

- Read the complete resume and job description. Ask for either only if missing and unavailable from the requested source. If several resumes are equally plausible, ask which to use.
- Treat the supplied resume and explicit user corrections as the factual baseline. Do not silently import stale career details from memory.
- Preserve section names and order, role order, bullet counts per role, headings, dates, employers, official job titles, and contact information unless the user explicitly supplies corrections or authorizes structural changes.
- Preserve Markdown conventions or DOCX styles, tables, fonts, spacing, margins, and layout. Keep edited text near the original length to avoid pagination changes.

## Tailoring workflow

1. Extract the job's core responsibilities, required skills, preferred skills, technical terminology, and expected scope of ownership.
2. Map each requirement to evidence in the resume or user-provided context. Distinguish demonstrated experience from transferable experience and unconfirmed gaps.
3. Rewrite the responsibilities and achievements of current and previous roles to emphasize the strongest relevant evidence. Use present tense for ongoing responsibilities and past tense for completed achievements and previous roles.
4. Use concise action-led bullets: action, relevant technical or business context, and supported outcome. Preserve verified metrics and scope. Reorder bullets within a role when it improves relevance without changing the structure.
5. Tailor existing summary, skills, and project sections when useful. Incorporate exact job-description keywords naturally where they accurately describe the candidate's experience; expand relevant acronyms where space permits.
6. Optimize assertively through wording, emphasis, and specificity. Do not invent employment, qualifications, technologies used, responsibilities, metrics, or accomplishments. Put potentially useful unsupported additions in a separate confirmation list, outside the submission-ready resume. Complete all supported edits without waiting for optional confirmations.
7. Avoid keyword stuffing, hidden text, copied job-description paragraphs, and claims of guaranteed ATS success or fabricated ATS scores.

## File handling and validation

- Use the Library skill for retrieving and saving resume artifacts when available. By default, create a tailored copy and preserve the original; update the original only when requested.
- For `.md`, edit text in place within the existing structure and compare headings, roles, and bullet counts with the source.
- For `.docx`, use the documents skill and edit the existing document rather than rebuilding it. Render and inspect the final document; fix clipping, broken bullets, spacing problems, and unintended page-count changes before delivery.
- Return the same format as the input unless another format is requested. Use a descriptive name such as `Name_Resume_Company_Role.md` or `.docx`.
- Check that each new factual claim is supported, the most relevant supported keywords appear naturally, and preserved identity and employment fields remain intact.
- If the existing structure limits ATS readability, preserve it as requested and briefly explain the specific limitation rather than silently redesigning it.

## Delivery

Provide the completed resume file with a short description of the main changes. List only material gaps or claims needing confirmation, separately from the resume. Do not submit applications or send the resume to anyone unless explicitly instructed.