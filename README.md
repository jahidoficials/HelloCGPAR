# Hello CGPAR — Exact Reference Formatting Version

This version uses the two supplied reference letters as the formatting masters:

- `template_director.docx` → Director / Senior Analyst layout
- `template_deputy.docx` → Deputy Director layout

The generated Word letter preserves the reference document's:
- US Letter page size
- 1-inch margins
- exact top blank space before the date
- date alignment
- blank line after the date
- Head of HR placement
- bold company name
- address line spacing
- blank line before/after the Re line
- centered + bold Re line
- blank line before Dear Sir/Madam
- body paragraph spacing and justification
- exact bold student-name / ID / school formatting
- closing spacing
- signature block spacing
- official name/title/phone formatting

PDF is generated from the same DOCX using LibreOffice on Streamlit Community Cloud, so Word and PDF use the same layout engine.

## Files

- `app.py` — Streamlit app
- `template_director.docx` — Director reference formatting master
- `template_deputy.docx` — Deputy Director reference formatting master
- `students.json` — eligibility data
- `companies.json` — company/address data
- `requirements.txt` — Python dependencies
- `packages.txt` — Linux dependencies for LibreOffice/PDF conversion
- `fonts/` — Carlito fallback fonts

## Deployment

Keep the Streamlit entrypoint as `app.py`.

After replacing these files in GitHub, commit the changes. Streamlit Community Cloud will rebuild the existing app.

Do not rename `app.py`.
