# Zeest report workspace

Start with your own folder: **[kashaf/START_HERE.md](kashaf/START_HERE.md)**, **[fatima/START_HERE.md](fatima/START_HERE.md)** or **[esha/START_HERE.md](esha/START_HERE.md)**. Each contains your files, first tasks, dependencies and an agent prompt.

Current submission: **Deliverable II, R&D, Chapters 1 through 6**, with compulsory Abstract, Executive Summary and References, plus the user-selected Appendix. Chapters 7 through 10 are archived outside the repository and are not assembled for this submission. The six chapters and compulsory front matter have been integrated. The prototype is unbuilt; interface images are design mockups and no empirical results are claimed.

## Folder map

| Location | Purpose |
|---|---|
| `kashaf/` | Chapters 1, 2, 4, Appendix, Executive Summary, own references and diagram sources |
| `fatima/` | Chapters 3, 5, Abstract, own references and diagram sources |
| `esha/` | Chapter 6, own references and diagram sources |
| `Report template/` | Frozen main assembly, untouched class, original reference examples and required Figures folder |
| `PLAN.md`, `Rules.txt` | Detailed required headings, diagrams, workload, defense questions and formatting |
| Proposal and `Sample Reports/` | Shared source documents; proposal alone defines project facts |

Every member keeps their coordination notes in their own `HANDOFF.md`. PlantUML sources go in their own `diagrams/`; rendered assets go in `Report template/Figures/` with `kashaf_`, `fatima_` or `esha_` prefixes. Captions must describe images accessibly. Do not invent prototype screenshots; tables stay LaTeX text. Use PLAN.md for alternatives where PlantUML is unsuitable.

## Project facts and boundaries


The only authoritative project source is [F26-098.docx](F26-098.docx); the supplied [PDF](F26-098.pdf) is its reading companion. Advisor: Miss Umm-e-Ammarah. The user confirmed the current six-chapter R&D Deliverable II scope. Rules.txt names FYP-1. Ownership is approved: Kashaf/A, Fatima/B and Esha/C.

Zeest proposes a physician-controlled, multimodal clinical decision support prototype with longitudinal relational and semantic patient memory. Its nine proposal objectives cover:

1. Hybrid relational and semantic patient memory.
2. Real-time consultation transcription into structured notes.
3. Patient Memory, Clinical Case, Imaging, Laboratory and Medication Safety agents.
4. Integration of an existing validated pre-trained imaging classification model.
5. Evidence and RAG retrieval of relevant guidelines with citations.
6. Clinical Reasoning output of a reviewable proposed diagnosis; scope also includes physician-reviewed treatment plans.
7. Safety and Critic review before presentation.
8. Physician approval, modification or rejection and a full audit log; approval is required before recording a clinical decision.
9. Ablation comparing a single LLM, a memory-augmented variant and the full system. The Introduction also asks about critic and multimodal contributions.

The proposal names FastAPI, Next.js, LangGraph, Google ADK, Gemini, PyTorch, PostgreSQL and pgvector. It discusses MIMIC-IV/MIMIC-CXR, PubMed, Synthea and imaging dataset/model candidates. Names in the proposal do not establish approved data access, a final model/domain selection or a completed integration. Do not invent the LangGraph/ADK division, hardware, numerical targets, languages, reviewers, sample counts or reference labels.

Use de-identified or synthetic data and supported domains with both suitable data and validated models. Exclusions include training diagnostic models from scratch, autonomous treatment/prescribing, real clinical deployment, regulatory approval, unsupported domains, patient chat/mobile apps, knowledge graphs and emergency/ICU systems. `context.txt` is old brainstorming, **not** an authoritative project specification. Sample reports guide presentation only; their headings, claims, results and citations do not override this template or become Zeest facts.


## Shared writing rules

Read `AGENTS.md`, `PLAN.md`, `Rules.txt`, the proposal and template before writing. Keep required chapter/section order and titles. Never edit `FastFyp.cls` or add packages. `main.tex` now assembles only Chapters 1 through 6, References and Appendix under the explicitly approved scope update. It is frozen again. Title-page metadata and declaration names are populated. BS(CS) and 10 October 2026 are integration assumptions requiring team confirmation; signature spaces remain blank.

Ordinary substantive prose: one concise 150--250-word paragraph per substantive heading under the feedback revision. Brief table introductions, captions, table cells and feature bullets are exempt. Abstract: one paragraph, 50?125 words, three to five sentences. Executive Summary: approximately one page of plain paragraphs, each within 150--250 words. Refer to every figure; use descriptive captions, automatic numbering and citations. Literature review needs at least 15 distinct verified relevant works.

Use normal design and requirement wording for prospective implementation and evaluation. The user approved removal of red PLANNED markers; preserve their status information without claiming completed work. Never invent references, results, resources or data access. Original bibliography examples are preserved in Report template/fypbib.bib but are not assembled into the project bibliography. Use citation prefixes `zeestA:`, `zeestB:`, `zeestC:` and one canonical owner for shared sources.

## Working together

Use separate clones and branches, one owner per file:

```powershell
git clone https://github.com/Kashaf-471/fyp-report.git
cd fyp-report
git switch -c report/kashaf
# Other members use report/fatima or report/esha.
```

Fetch and merge the actual shared branch before new work. Review each other's changes through PRs; do not edit another person's files. Read each person's HANDOFF.md before using their decisions. Requirements, methodology, design and planned tests must agree before finalizing. Write summaries last. Root documents and assembly changes require a separate agreed coordinator task. Never force-push shared history.

## Compile

Compile from **Report template/** so existing class and figure paths resolve. Keep all three sibling person folders when uploading to Overleaf and select `Report template/main.tex` as the main document. Use a standard TeX installation with the class's existing dependencies:

```powershell
cd 'Report template'
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

These pdfLaTeX commands require an installed TeX distribution and have not been verified locally. The local verification uses Tectonic/XeTeX. The earlier full-template relocation matched all 39 original pages at 144 DPI. The current six-chapter assembly intentionally differs from that original; XeTeX substitutes unavailable Times font shapes; intended typography still needs validation. Existing template SDG-reference, header-height and box warnings remain. No font/package fixes were made.

Generated PDFs and auxiliary files are ignored by Git. Required figure assets remain tracked.

## Setup archive

The old `.phase2`, `baseline` and verification machinery is no longer in this repository. Original template sources/PDF, setup audit and local tools are preserved on the coordinator's machine at `D:\Codes_shit\Fyp Report setup archive 2026-10-04`. Team members do not need this archive to write or use a standard TeX toolchain. Its old scripts record the former layout and are historical rather than the current build interface.

Approved report integration is complete. Resource selection, implementation and executed evaluation remain future work. No commit or push was performed during finalisation.

## Deliverable II dependencies

Kashaf supplies proposal scope, objective/requirement IDs, use-case meanings and the proposed data dictionary. Fatima verifies literature and defines methodology and planned evaluation contracts. Esha aligns the architecture and detailed design with both. Esha owns one chapter with six planned design diagrams, Fatima carries literature verification, and Kashaf carries the requirements tables and proposed interface views. Write Abstract and Executive Summary after the six chapters agree. Appendix A contains objective traceability and configuration decisions; unrelated template demonstrations have been replaced.

Kashaf requests explicit approval at every step and reviews two chapters together. For Kashaf, outline in chat, get approval, draft in chat, then obtain explicit approval before saving. Use Zeest with a capital Z and no em dashes in Kashaf's authored text. These personal style preferences do not grant permission to rewrite other members' work.

## Final integration, 10 October 2026

The user authorised this task-specific exception to member ownership and frozen assembly restrictions. Member ownership and main.tex freezing resume after this integration. FastFyp.cls was not edited and no packages were added. The required chapter order and front-matter items are retained; instructional database-heading text and demonstration literature/appendix headings have been replaced with project headings under the approved plan.

Compile from Report template/. The reviewed local PDF is `Report template/build/Zeest-An-Agentic-Medical-Copilot-FYP-I.pdf`; generated build output stays ignored. Upload the full repository structure to Overleaf, with Report template/main.tex selected as the main document.

The build uses the original class's Times fonts and spacing. Local main.tex font-encoding commands restore Times under XeTeX, and header height is compensated to keep the text-body position unchanged. Declaration spacing was reduced so both declarations fit together. Automatic contents, figure/table lists and IEEE references are regenerated. Both physician navigation diagrams are retained.

## Feedback revision, 10 October 2026

The user authorised the full-report feedback fixes and a longer Executive Summary. The summary is one page with two plain paragraphs (177 and 170 words). Chapters 2, 4 and 6 now have numbered conclusions, preserving all existing required headings. Stakeholders Summary is prose. The literature summary uses a larger font, the requested caption and an explicit float boundary before its conclusion.

GUI images use larger typography and exports measured to fit their actual content. Suitable frames share a page at full width; longer screens remain separate for readability. Both navigation views remain. Wide diagrams use enlarged, rotated illustrations through the class's existing graphicx support; A4 page size and margins are retained. Design diagrams use vector PDFs, and the domain model is monochrome. Editable PlantUML/SVG sources stay in esha/diagrams/ and report-ready assets in Report template/Figures/.

The sharper Goal 3 image is the official UN icon; the original grid asset remains preserved. The template-required SDG heading and use-case diagram remain despite generic feedback that conflicts with the supplied template. Declaration signatures must be supplied by the students; no signatures or empirical results were invented.
