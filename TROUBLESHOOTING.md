# Troubleshooting (common LaTeX errors)

If your CV stops compiling after you edited `EDIT_ME.tex`, it is almost always one of these:

---

## 1) "Missing } inserted" or "Runaway argument"

You accidentally removed a curly brace.

**Fix:**
- Look at the last place you edited.
- Make sure every `{` has a matching `}`.
- A fast test: undo your last change and recompile.

---

## 2) "Undefined control sequence"

This usually happens when you typed a backslash command that LaTeX doesn't recognize.

Common causes:
- You typed `\n` or `\t` like in programming languages.
- You misspelled a command, e.g. `\resumSubheading` (typo).

**Fix:**
- Remove the unknown command or copy/paste from an existing working block.

---

## 3) "LaTeX Error: File `____.sty` not found"

A package is missing from your local LaTeX installation.

**Fix options:**
- Use Overleaf (recommended; it includes most packages).
- Or install missing packages via your LaTeX distribution.

---

## 4) Links or icons look weird

If you delete only part of a link/icon line, the spacing may look odd.

**Fix:**
- Delete the whole item (icon + link) or leave the URL blank.

Example (hide Google Scholar):

```tex
\newcommand{\CVScholarURL}{}
```

---

## 5) "There's too much content on one page"

This template is tuned for concise CVs/resumes.

**Fix options:**
- Remove less important bullets.
- Shorten bullet text.
- Remove optional sections (Projects / Publications / Awards).
- Adjust margins or font size (advanced): edit `cv_style.tex`.
