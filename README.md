# IIM-associated cancer screening (single-page)

Clinician-facing prototype: a 1-page React tool for IIM-associated cancer screening recommendations based on structured risk logic.

## Run locally

This is a single static `index.html` that loads React from an ESM CDN.

- Open `index.html` directly in a browser, **or**
- Serve the folder (recommended) to avoid any browser module/CORS restrictions:

```bash
python3 -m http.server 5173
```

Then visit `http://localhost:5173`.

## Notes

- Juvenile-onset IIM and inclusion body myositis (IBM): output states “Cancer screening not routinely required” and hides the adult risk factor calculator.
- Adult-onset IIM: toggles risk factors, computes high/intermediate/low counts, and applies the risk stratification logic exactly as specified.
- Optional: “Geographic region with increased risk of nasopharyngeal carcinoma” adds a note to consider nasoendoscopy at diagnosis.

