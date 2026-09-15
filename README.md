# Course Notes to Presentation

把课程笔记、视频字幕、访谈稿、读书笔记或已有 PPT，整理成可信、生动、可直接使用的 PPT 文案和逐页演讲稿。

The skill turns course notes, lecture transcripts, interviews, reading notes, or an existing deck into source-aware slide copy and a page-aligned speech script. It also supports timed, bilingual English classroom presentations.

## What it adds

- separates source facts, speaker opinions, reasonable inference, and uncertainty;
- writes exact on-screen words instead of vague slide suggestions;
- uses stories, reasoning questions, audible signposts, and a recurring theme;
- keeps PPT speaker notes, scripts, translations, and timing synchronized;
- estimates English word count from the required duration;
- defaults to simple A2–B1 spoken English for general classroom talks;
- requires rendered slide and document checks when actual files are created.

## Install

### Codex on Windows PowerShell

If `CODEX_HOME` is configured:

```powershell
git clone https://github.com/yui-research/course-notes-to-presentation.git "$env:CODEX_HOME\skills\course-notes-to-presentation"
```

If it is not configured, clone into your personal Codex skills folder:

```powershell
git clone https://github.com/yui-research/course-notes-to-presentation.git "$HOME\.codex\skills\course-notes-to-presentation"
```

Restart Codex after installation if the skill is not discovered immediately.

### macOS or Linux

```bash
git clone https://github.com/yui-research/course-notes-to-presentation.git "${CODEX_HOME:-$HOME/.codex}/skills/course-notes-to-presentation"
```

## Use

Invoke the skill explicitly:

```text
Use $course-notes-to-presentation to turn these course notes into a 10-slide presentation and a page-aligned speech script.
```

English classroom example:

```text
Use $course-notes-to-presentation to create an 8–10 minute English classroom presentation. Keep the slides minimal, use simple spoken English, provide a Chinese translation, and synchronize the PPT notes with the final script.
```

The skill also allows implicit invocation when the request clearly matches its purpose.

## Repository structure

```text
course-notes-to-presentation/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── english-classroom-delivery.md
    ├── output-contract.md
    ├── voice-and-storytelling.md
    └── worked-example.md
```

## Publish this repository

Create an empty repository on GitHub or Gitee. Do not initialize it with another README, `.gitignore`, or license. Then run these commands inside this folder:

```bash
git remote add origin https://github.com/YOUR-NAME/course-notes-to-presentation.git
git branch -M main
git push -u origin main
```

Replace `YOUR-NAME` and the remote URL with your own account and repository address.

## License

No license is included yet. Before public release, choose a license that matches how you want others to reuse and modify the skill. MIT is a common permissive choice for reusable skill repositories.

## Contributing

Issues and pull requests are welcome. Keep changes general-purpose, preserve evidence boundaries, and do not add private course files or copyrighted transcripts to the repository.
