# Tu Li’s Personal Website and CV

This is the central guide for updating my personal academic website and CV. Keep it beside `docs` and `cv_sept26`, and update it when their files or maintenance steps change.

Updated September 8, 2026.

- **Public website:** [tuliecon.github.io](https://tuliecon.github.io)
- **GitHub repository:** [tuliecon/tuliecon.github.io](https://github.com/tuliecon/tuliecon.github.io)
- **Website files on GitHub:** [open the docs folder](https://github.com/tuliecon/tuliecon.github.io/tree/main/docs)
- **Local project folder:** `C:\Users\tuli8\Desktop\personal_website`
- **Website working folder:** `docs`
- **Editable CV source:** `cv_sept26/cv.tex`
- **Publishing settings:** branch `main`, folder `/docs`.

The website uses four ordinary HTML pages and one stylesheet, which can be edited and previewed without installing software. The CV is an ordinary LaTeX document: edit `cv_sept26/cv.tex` and compile it with pdfLaTeX to produce `cv_sept26/cv.pdf`. The website serves a separate copy at `docs/cv.pdf`.

## My usual update workflow

**Ask for changes → review locally → commit and push to GitHub → check the public website.**

Keep using this `personal_website` folder. To make changes and publish them, ask **“Update and publish my website”** and describe the changes. The assistant will:

1. Fetch the latest GitHub revisions and reconcile them with any local edits before making changes. Tell the assistant if I have also edited or uploaded files directly on GitHub.
2. Edit the intended files in `docs` and update this guide when needed. For a CV update, edit and compile the local source, review it, and copy the finished PDF into `docs/cv.pdf`.
3. Preview the changed pages and check their links and PDFs. I can also double-click `docs/index.html` to preview the website myself.
4. Review the changed files, commit the intended changes, and push `main` to GitHub. A commit saves a local revision; a push sends that revision to GitHub.
5. Check the latest deployment in [Actions](https://github.com/tuliecon/tuliecon.github.io/actions) and the public pages and PDF links. If an older version appears, press **Ctrl + F5**.

Local saves, previews, and commits alone do not publish anything. The push triggers GitHub Pages to publish the website. If I only ask for local edits, they remain local until I ask to publish. Local files and GitHub do not synchronize automatically.

### Git connection on this computer

This folder is connected to `https://github.com/tuliecon/tuliecon.github.io.git`; local branch `main` tracks `origin/main`. Git is installed at `C:\Program Files\Git\cmd\git.exe`. If an already-open terminal does not recognize `git`, reopen it or use that full executable path. The repository uses the commit name **Tu Li** and GitHub's noreply address to keep the personal email private. Git Credential Manager is bundled with Git and can open a browser for GitHub sign-in when authentication is needed; complete that sign-in with the `tuliecon` account.

The Git ignore rules allow new tracked content only in `docs`, this `README-PERSONAL-WEBSITE.md`, and `.gitignore`. The editable CV source, `cv_sept26`, `backups`, `tmp`, and other files outside that list stay local. This single guide replaces the old two-line `README.md` and is the canonical maintenance reference.

**Git setup completed September 7, 2026:** connected and signed in as `tuliecon`; publishing access was verified. To check whether the latest changes are live, compare the local Git status with `origin/main` after fetching, then check the deployment in Actions and the public website.

## Manual upload fallback

I can still publish through GitHub's browser upload if needed. First make sure the local files include any recent GitHub edits. Open the matching destination folder from the table below, click **Add file → Upload files**, and drag in the changed files. To select several files in Windows, hold **Ctrl** while clicking them. Enter a short message such as **Update website**, select **Commit directly to the main branch**, and click **Commit changes**. Wait for deployment in Actions and check the public website. Before the next Git update, tell the assistant about these browser changes so it can fetch and reconcile them.

### Upload files into the correct folder

GitHub places uploaded files into the folder open when I select **Add file → Upload files**. For example, to update Home and Research, first open [docs on GitHub](https://github.com/tuliecon/tuliecon.github.io/tree/main/docs), then upload just `index.html` and `research.html` from my local `docs` folder. This updates `docs/index.html` and `docs/research.html`.

When already inside `docs` on GitHub, upload the files themselves. Dragging the whole `docs` folder here would create an unwanted `docs/docs` folder.

| What I am uploading | Folder to open on GitHub first | What to drag from my computer |
|---|---|---|
| Home, Research, Teaching, or Notes edits | `docs` | The changed HTML files |
| A new CV | `docs` | `cv.pdf` |
| A replacement paper PDF | `docs/papers` | The PDF itself |
| A replacement ECON 453 PDF | `docs/econ453` | The PDF itself |
| A replacement ECON 330 PDF | `docs/econ330` | The PDF itself |
| The stylesheet | `docs` | `style.css` |
| My replacement photo | `docs/files` | `tuli.jpg` |
| A new folder of notes or course materials | `docs` | The new folder |
| The entire updated website | Repository's main file list, outside `docs` | The whole `docs` folder |

### Upload the entire docs folder instead

If my local copy is current, I can upload the entire website. Start at [the repository's main file list](https://github.com/tuliecon/tuliecon.github.io), where the existing `docs` folder is visible. Click **Add file → Upload files**, drag the whole local **docs folder**, and commit to `main`. Upload paths should start with one `docs/`, such as `docs/index.html`.

Files with the same folder path and filename update their existing versions. New names add new files. Files missing from the upload are not deleted from GitHub. If an old file's public URL has been shared, keep that file available even after giving its replacement a new name.

The upload controls are documented in [GitHub's file upload guide](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository).

## Website files and current contents

All paths below are inside the local `docs` folder.

| File or folder | What it contains |
|---|---|
| `index.html` | Home: fifth-year PhD introduction, research interests, current working paper link, email, photo, and CV link. The biography begins directly, with no greeting heading; education before the PhD is omitted. Browser title: "Tu Li \| Economics PhD Student, University of Arizona." |
| `research.html` | Working paper title, abstract, and **[Draft]** link to `papers/sms.pdf`; two abandoned projects with abstracts, **(No longer active)** labels, and separate **[Draft]** PDF links. |
| `teaching.html` | One compact entry per course: **ECON 453: Data Analytics and Modeling: Quantitative Analysis for Economic Strategy**, **Fall 2026; Spring 2026**, with both syllabi, **Evaluation (Spring 2026)**, and Slides 1-14; **ECON 330: Macroeconomic and Global Institutions and Policy**, **Summer 2026; Summer 2025**, with both syllabi. |
| `econometrics-notes.html` | "Notes will be added here." No note PDFs yet. |
| `style.css` | Appearance shared by all four pages. |
| `cv.pdf` | The CV linked from Home. |
| `files/tuli.jpg` | Homepage photo. |
| `papers/` | Research PDFs listed below. |
| `econ453/` | 17 linked teaching PDFs: Fall 2026 and Spring 2026 syllabi, Spring 2026 evaluation, and Slides 1-14; plus the legacy `syllabus_tu.pdf` copy to preserve its public URL. |
| `econ330/` | 2 teaching PDFs: Summer 2026 and Summer 2025 syllabi. |
| `.nojekyll` | Marker for publishing ordinary HTML; keep this file. |

The folders `cv_sept26`, `backups`, and `tmp` are outside the published website and excluded from Git. Original CV source material is kept in `cv_sept26/archive`; use `cv_sept26/cv.tex` for current edits. The CV instructions below are maintained here together with the website instructions.

All pages share the same navigation: Home, Research, Teaching, Econometrics Notes. The CV is linked from Home. If I ever change the navigation, I need to update it in all four HTML files.

## Update my CV

| File | Purpose |
|---|---|
| `cv_sept26/cv.tex` | Editable LaTeX source; make CV changes here. |
| `cv_sept26/cv.pdf` | PDF produced by compiling the source; review this version first. |
| `docs/cv.pdf` | Website copy; replace it with the reviewed PDF when ready. |
| `cv_sept26/archive/` | Original source material kept for reference. |

### Edit the LaTeX source

Open `cv_sept26/cv.tex` in a text editor. The visible content is written directly after `\begin{document}`: edit the name, contact details, update date, dates, titles, course terms, and descriptions where they appear. There are no custom CV commands to fill in.

- To add an entry, duplicate a complete nearby entry block, including its formatting, and change the text. For another teaching semester, append it to that course's existing term line, separated by a semicolon.
- To add a section, copy an existing `\section*{...}` heading and a suitable entry block; change the heading and content. For example, use `\section*{Research in Progress}` when ready to add those projects.
- To remove a section, delete its heading and entries up to the next section heading. Keep `\begin{document}`, `\end{document}`, and matching braces and environment boundaries.
- A line beginning with `%` is an editing comment and does not appear in the PDF. In ordinary text, write `\&`, `\%`, `\_`, `\#`, and `\$` to display those special characters; write `\{` and `\}` for literal braces. Keep existing LaTeX commands and table separators intact.
- Contact links use ordinary LaTeX link commands. If changing an email or website, update both the destination and displayed text when both are present. Paper titles and abstracts can remain plain text.

### Compile and review

Open PowerShell and run these commands. pdfLaTeX is installed on this computer; on another computer, install a LaTeX distribution or use Overleaf below.

```powershell
Set-Location -LiteralPath 'C:\Users\tuli8\Desktop\personal_website\cv_sept26'
pdflatex -interaction=nonstopmode -halt-on-error cv.tex
pdflatex -interaction=nonstopmode -halt-on-error cv.tex
```

After both runs succeed, open `cv_sept26/cv.pdf` and review every page for correct content, dates, spacing, and page breaks. If compilation fails, correct the reported error before copying the PDF to the website; an existing PDF may still be the previous version. The paper size is US Letter; change `letterpaper` to `a4paper` in `\documentclass` only if an A4 version is needed.

Alternatively, upload `cv.tex` to an Overleaf project, select **pdfLaTeX** as the compiler, and click **Recompile**. After editing there, save the updated `cv.tex` back into local `cv_sept26` and download the resulting PDF as `cv_sept26/cv.pdf`. This keeps the local source and PDF together.

### Publish the reviewed CV

1. Copy the reviewed `cv_sept26/cv.pdf` into the local `docs` folder, replacing **docs/cv.pdf**.
2. Ask the assistant to publish the reviewed CV using the usual Git workflow. For the manual fallback, upload the replacement `cv.pdf` itself from inside [docs on GitHub](https://github.com/tuliecon/tuliecon.github.io/tree/main/docs).
3. After the push or browser commit, wait for deployment and check [the public CV](https://tuliecon.github.io/cv.pdf).

Compiling the CV does not automatically update `docs/cv.pdf` or GitHub. Copying it to `docs` prepares the local website; publishing requires a Git push or browser upload and commit. Keeping the filename `cv.pdf` preserves the homepage link without an HTML edit. If CV changes also affect the homepage biography, research page, or teaching page, include those HTML changes in the publication.

## Update or add a research paper

Paper titles are plain text. Available files are linked separately as **[Draft]**, **[Slides]**, or **[Replication]** in a `<span class="paper-links">...</span>` immediately after the title and any status label. The two abandoned papers keep **(No longer active)** and currently have only **[Draft]** links.

The current PDF filenames are:

| Paper | File in the local docs folder |
|---|---|
| Penalized and Debiased GMM with Potentially Invalid Moment Conditions | `papers/sms.pdf` |
| Weighted Regularization in Fixed Effects Panel Model: Convergence Rate and Oracle Property | `papers/sparse_fixed_effects.pdf` |
| The Impact of Electrification on Labor Productivity: Evidence from the Early 20th Century United States | `papers/electrification.pdf` |

To replace a PDF, keep its filename, replace the local copy, then publish using the usual workflow. To change a title, abstract, or status label, include edits to `docs/research.html` too. For manual uploads, the PDFs belong inside `docs/papers` on GitHub.

### Update the moment selection draft

**Penalized and Debiased GMM with Potentially Invalid Moment Conditions** appears under Working Paper, with the title and full abstract copied from my CV and a separate **[Draft]** link to `docs/papers/sms.pdf`.

The permanent latest-draft URL is [https://tuliecon.github.io/papers/sms.pdf](https://tuliecon.github.io/papers/sms.pdf). Keep the public filename `sms.pdf` for every revision so existing shared links serve the latest published draft.

1. Optionally keep a dated copy of the previous draft outside `docs`, such as `backups/papers/sms_2026-09-08.pdf`, using that draft's date. These archive copies stay local.
2. Replace `docs/papers/sms.pdf` with the updated PDF and review it.
3. Publish the replacement using the usual Git workflow, then check the public **[Draft]** link after deployment. The existing **[Draft]** link stays the same; edit `research.html` only if its text also needs updating.

The Research heading and draft link are:

```html
<h3 id="moment-selection-paper">Penalized and Debiased GMM with Potentially Invalid Moment Conditions <span class="paper-links"><a href="papers/sms.pdf">[Draft]</a></span></h3>
```

The homepage continues to link to the description using `research.html#moment-selection-paper`. Keep that heading's `id`. If the paper title changes, update its wording on both Home and Research.

For another paper, copy a complete `<article>...</article>` block into the appropriate Research section. Change the plain-text title, abstract, and separate file links. Give the heading a unique `id`, and use that same value in the article's `aria-labelledby`. Use an abandoned-project status label only for projects I no longer work on. Add a file link once the file exists.

To add slides or replication materials, save the actual files in `docs/papers` and append links inside the same `paper-links` span. For example, once all three example files exist:

```html
<span class="paper-links"><a href="papers/sms.pdf">[Draft]</a> <a href="papers/sms_slides.pdf">[Slides]</a> <a href="papers/sms_replication.zip">[Replication]</a></span>
```

Use the real filenames, or the full address of an existing external resource. Publish the changed `research.html` and new files together, preserving their paths under `docs/papers`. Do not add empty links or links to files that are not ready.

### Share a paper with others

Click **[Draft]** beside a paper on the live Research page and copy the PDF's address from the browser to share in an email or presentation. For the moment selection paper, use the [permanent latest-draft link](https://tuliecon.github.io/papers/sms.pdf). In a LaTeX document using `hyperref`, the same link is `\href{https://tuliecon.github.io/papers/sms.pdf}{Click here for the latest version}`. A file path on my computer is only a local preview. Replacing a published PDF at the same path keeps its shared address working and serves the new version.

## Update teaching materials or add a course

Teaching has one compact entry per course, with semesters and syllabus links ordered newest first. There are 19 downloads: 17 for ECON 453 and 2 for ECON 330. The syllabus paths inside local `docs` are:

| Course and semester | Syllabus file |
|---|---|
| ECON 453, Fall 2026 | `econ453/econ453_syllabus_fall_2026.pdf` |
| ECON 453, Spring 2026 | `econ453/econ453_syllabus_spring_2026.pdf` |
| ECON 330, Summer 2026 | `econ330/econ330_syllabus_summer_2026.pdf` |
| ECON 330, Summer 2025 | `econ330/econ330_syllabus_summer_2025.pdf` |

The syllabus links include their semesters, such as **Syllabus (Fall 2026)**. The ECON 453 evaluation remains `econ453/econ453_evaluation_spring26.pdf`, labeled **Evaluation (Spring 2026)**; its 14 slide filenames are unchanged. Replacing a PDF for the same semester means keeping its exact filename in `docs/econ453` or `docs/econ330` and publishing the replacement.

To publish teaching changes, ask the assistant to use the usual Git workflow for the changed `teaching.html` and PDFs in `econ453` and `econ330`. After deployment, check the two course entries and all download links. For the manual fallback, upload `teaching.html` and the affected course folders together from inside `docs` on GitHub. Future edits remain local until pushed or uploaded and committed.

The Fall 2026 syllabus now uses `econ453_syllabus_fall_2026.pdf`. The identical legacy copy at `docs/econ453/syllabus_tu.pdf` is also retained locally and on GitHub to preserve a previously shared public link. Keep that legacy file when committing future updates; it is additional to the 19 downloads linked from Teaching.

Filenames are case-sensitive online. Preserve the uppercase letters in `lecture6_OLS.pdf`, for example. Keep slide links in numerical order. If I change a PDF's name or the term it describes, update the corresponding link or label in `teaching.html` too. The existing evaluation is specifically labeled **Spring 2026**.

For another semester of an existing course, keep the older syllabus files and add a new PDF using `econ<course>_syllabus_<semester>_<year>.pdf`, with lowercase text and underscores. Add that semester to the same course entry and add its dated syllabus link, newest first; do not create a separate course entry or overwrite a previous semester's syllabus. Publish the changed `teaching.html` and new course PDF together.

To add a course:

1. Create a new folder inside local `docs`, such as `econ454`, and put its course PDFs there.
2. In `teaching.html`, copy the complete ECON 453 course block from `<section class="course" ...>` through its closing `</section>`. Paste it after the existing course entries.
3. Change the course title, semesters, and download links. Keep semesters and syllabus links newest first; add or remove links to match the supplied PDFs.
4. In the copied block, change both `id="econ453-title"` and `aria-labelledby="econ453-title"` to the same new value, such as `econ454-title`. Change `aria-label="ECON 453 downloads"` to the new course number.
5. Keep `download` on course links, for example:

```html
<li><a href="econ454/econ454_syllabus_spring_2027.pdf" download>Syllabus (Spring 2027)</a></li>
```

6. Preview the page, then publish the changed `teaching.html` and the new course folder together using the usual workflow.

## Add econometrics notes

1. Create a local `docs/notes` folder and put the note PDFs there.
2. In `econometrics-notes.html`, replace the placeholder paragraph with links using the actual filenames, for example:

```html
<p><a href="notes/my-first-note.pdf">My first note (PDF)</a></p>
```

3. Preview the page, then publish the changed `econometrics-notes.html` and the `notes` folder together using the usual workflow.

## Publishing settings and quick troubleshooting

The repository is already set up to publish from **Settings → Pages → Deploy from a branch → main → /docs**. Keep these settings for normal updates. GitHub publishes changes that reach this source through a push or browser commit. [GitHub Pages instructions](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

Keep `docs/.nojekyll`; it lets GitHub serve this ordinary HTML website without Jekyll processing. Include it in the next Git publication. For the manual fallback, if it is missing on GitHub, open `docs`, choose **Add file → Create new file**, name it `.nojekyll`, enter one blank line, and commit.

| What happened? | What to check |
|---|---|
| The website still shows the previous text or PDF | Confirm the commit reached GitHub through a push or browser commit, wait for deployment in Actions, then press Ctrl + F5. |
| Git asks me to sign in | Complete Git Credential Manager's browser sign-in with the `tuliecon` account, then retry publishing. |
| A push is rejected because GitHub has newer changes | Ask the assistant to fetch and reconcile the changes, then retry. Do not force-push over newer work. |
| A PDF link says 404 or file not found | Compare the link's filename, capitalization, and folder with the actual uploaded file. |
| My HTML files landed in the repository's root | Re-upload them from inside `docs` on GitHub; the website publishes that folder. |
| I accidentally created `docs/docs` | Upload the intended files into the first `docs` folder, verify the public site, then remove the accidental nested copies. |

Keep **README-PERSONAL-WEBSITE.md** beside `docs` as the single maintenance guide and include its updates in Git commits. It belongs at the repository root, so it does not become a page on the published website. Do not create a second root README with duplicate instructions.
