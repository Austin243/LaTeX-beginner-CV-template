# Beginner-Friendly LaTeX CV Template

This template is set up so beginners only edit one file:

- Edit `EDIT_ME.tex`
- Compile `main.tex`
- Leave `cv_style.tex` alone unless you want to change the design

You can open `preview.pdf` to see the example output.

## Overleaf Setup (Upload ZIP, easiest)

1. Go to Overleaf and sign in.
2. Click `New Project` -> `Upload Project`.
3. Upload `BeginnerFriendly_CV_Template.zip`.
4. Open `EDIT_ME.tex` and replace placeholders with your own details.
5. Click `Recompile` to build the PDF.
6. Download your PDF from `Menu` -> `Download PDF`.

## Overleaf Setup (Drag/Drop Unzipped Files)

Use this if you already unzipped the template and want to upload files manually:

1. Create a new blank project in Overleaf.
2. Drag these files into the Overleaf file tree:
   - `main.tex`
   - `EDIT_ME.tex`
   - `cv_style.tex`
   - `assets/ieee_collabratec_icon.png`
3. If Overleaf does not auto-create the folder, create an `assets` folder and upload the icon there.
4. In Overleaf `Menu`, set `Main document` to `main.tex`.
5. Recompile.

## Local Compile (Optional)

If you already have a LaTeX installation:

```bash
pdflatex main.tex
pdflatex main.tex
```

## Important Files

- `README_START_HERE.md`: detailed beginner walkthrough
- `TROUBLESHOOTING.md`: common LaTeX errors and fixes
- `LICENSE_AND_CREDITS.md`: author and license summary
