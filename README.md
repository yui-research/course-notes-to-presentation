# Course Notes to Presentation

> Turn course notes, lecture transcripts, video subtitles, interviews, reading notes, or an existing PPT into a clear slide deck and a timed, page-aligned speech script.

把课程笔记、课堂讲义、视频字幕、访谈稿、读书笔记或已有 PPT，整理成简洁可信的幻灯片文案、逐页演讲稿和中英双语课堂汇报。

## 适用场景 / Use cases

- 课程汇报与学术分享 / classroom and academic presentations
- PPT、PowerPoint 与 slide deck 文案 / slide copy and deck structure
- 8–10 分钟英语演讲 / timed English presentations
- 演讲稿、speaker notes 与中文译文 / speech scripts, speaker notes, and Chinese translations
- 故事引导、现场提问、语言标记和主题回环 / storytelling, audience questions, signposts, and theme callbacks

## 快速开始 / Quick start

```text
Use $course-notes-to-presentation to turn these notes into a concise PPT and an 8–10 minute page-aligned speech script. Use simple English and provide a Chinese translation.
```

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

## Skill 简介

这是一个面向课程汇报和学术分享的 Codex Skill。它可以把课程笔记、视频字幕、访谈稿、读书笔记或已有 PPT，整理成可信、生动、控时且可直接使用的 PPT 文案和逐页演讲稿。

它尤其适合制作简洁的课堂 PPT、8–10 分钟英语汇报、中英双语讲稿，以及需要故事引导、主题回环、现场提问和语言标记的演讲。

This Codex Skill turns course notes, lecture transcripts, interviews, reading notes, or an existing deck into source-aware slide copy and a page-aligned speech script. It also supports timed, bilingual English classroom presentations.

## 核心能力

- separates source facts, speaker opinions, reasonable inference, and uncertainty;
- writes exact on-screen words instead of vague slide suggestions;
- uses stories, reasoning questions, audible signposts, and a recurring theme;
- keeps PPT speaker notes, scripts, translations, and timing synchronized;
- estimates English word count from the required duration;
- defaults to simple A2–B1 spoken English for general classroom talks;
- requires rendered slide and document checks when actual files are created.

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
├── LICENSE
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

This project is released under the [MIT License](LICENSE). You may use, copy, modify, and redistribute it under the license terms.

## Contributing

Issues and pull requests are welcome. Keep changes general-purpose, preserve evidence boundaries, and do not add private course files or copyrighted transcripts to the repository.
