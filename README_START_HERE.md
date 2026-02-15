# Beginner-Friendly CV / Resume Template (LaTeX)

This project is set up so that *beginners only edit one file*:

- ✅ **Edit:** `EDIT_ME.tex`
- ✅ **Compile:** `main.tex`
- ⚠️ **Do not edit (unless you want to change the design):** `cv_style.tex`

You can also open **`preview.pdf`** to see what the placeholder CV looks like.

---

## Option A: Use in Overleaf (recommended for beginners)

Overleaf (https://www.overleaf.com) is a website with an online LaTeX editor, so you can edit your CV in the browser.

1. Go to Overleaf and sign in (free account is fine).
2. Click **New Project** → **Upload Project**.
3. Upload the **.zip** that contains these files.
4. In the left file list, click **`EDIT_ME.tex`**.
5. Replace the placeholders with your own info.
6. Click **Recompile** (top right) to see the PDF update.
7. Download your PDF: **Menu** → **Download PDF**.

---

## Option B: Compile locally (if you already have LaTeX installed)

### Mac / Linux (TeX Live)
In the folder with `main.tex`:

```bash
pdflatex main.tex
pdflatex main.tex
```

### Windows
Install **MiKTeX** or **TeX Live**, then run the same commands (or compile via your editor).

---

## What to edit

### 1) Your name + contact info
Open `EDIT_ME.tex` and edit the block at the top:

```tex
\newcommand{\CVName}{YOUR NAME}
\newcommand{\CVPhone}{+1 (555) 123-4567}
\newcommand{\CVEmail}{you@example.com}
```

You can also leave a link blank to hide it:

```tex
\newcommand{\CVScholarURL}{}
```

### 2) Sections (Education, Experience, etc.)
To add another job/school, **copy + paste** an existing block and edit the text inside `{ ... }`.

Example education entry:

```tex
\resumeSubheading
  {University Name}{City, Country}
  {Degree}{Start Year -- End Year}
```

Example bullet list:

```tex
\resumeItemListStart
  \item Did something impressive
  \item Used numbers when possible (e.g., improved speed by 40\%)
\resumeItemListEnd
```

---

## Beginner "gotchas" (read this if you get errors)

### Curly braces must match
If you delete a `{` or `}`, LaTeX will usually fail to compile.

### Special characters must be escaped
If you need to type these characters literally, add a backslash:

- `50\%`
- `AT\&T`
- `my\_file`

Characters that need escaping:

`#  $  %  &  _  {  }  ~  ^  \`

### Commenting out lines
Putting a `%` at the start of a line hides it:

```tex
%\section{\textbf{Projects}}
```

---

## Sharing this template with others

The easiest way to share:

- **As a zip:** send the `.zip` file.
- **As an Overleaf project:** Overleaf → **Share** → copy the link.

If you plan to publish this publicly (Overleaf Gallery, GitHub, etc.), read **LICENSE_AND_CREDITS.md**.

---

## Paper size (A4 vs Letter)

This template defaults to **A4** paper. If you want **US Letter**, open `main.tex` and change:

```tex
\documentclass[a4paper,11pt]{article}
```

to:

```tex
\documentclass[letterpaper,11pt]{article}
```
