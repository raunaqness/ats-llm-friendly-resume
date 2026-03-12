# Resume Tailoring Workflow

This repo contains a LaTeX resume source (`resume.tex`) and generated PDF output.

## Repository Structure
- `resume.tex`: Main resume source file
- `resume.pdf`: Default generated PDF
- `resume-tailored-vertexai-devops.pdf`: Example tailored output
- `.gitignore`: Git ignore rules

## Prerequisites
- LaTeX engine: `tectonic` (recommended)
- Git
- Codex (or any editor/agent workflow)

## How to Use
1. Git clone this repository
2. Open on Codex (editor of your choice)
3. Use this prompt template:

```text
Tailor my Resume for the following JD:

<JD-Details>

Give me a diff of the changes before you generate the PDF.
```

4. Review the diff
5. If it looks good, generate the PDF

## Build PDF
From repo root:

```bash
tectonic resume.tex
```

To save a versioned output:

```bash
cp resume.pdf resume-tailored-<role>.pdf
```

## Recommended Codex Flow
1. Ask for JD-based tailoring with diff first
2. Confirm no inaccurate claims were introduced
3. Generate and review PDF
4. Commit updated `resume.tex` and selected PDF artifact

## Tips
- Keep claims evidence-based and interview-defensible
- Prefer role-specific keywords in Summary, Skills, and top 1-2 Experience sections
- Avoid stuffing keywords at the cost of readability
