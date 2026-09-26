## What does this PR do?
Add resource(s)

## IMPORTANT
- [x] Read our [contributing guidelines](https://github.com/EbookFoundation/free-programming-books/blob/main/docs/CONTRIBUTING.md).
- [x] Is this a revision of a previously submitted PR? If so, STOP! Go back, reopen the PR, and add commit(s) the branch you previously submitted. Please don't make the job of reviewing more difficult by hiding previous work.

  None of these are my own earlier PRs. This PR finishes resources that other people suggested in open issues and PRs, with the reviewers' requested changes applied. The original authors are credited below so those issues and PRs can be closed.

## For resources
### Description

Adds 16 entries across 11 files. They come from open issues and PRs that were stalled, stale, or had review changes nobody made yet:

| Source | Entry | File | Changes from the original |
|---|---|---|---|
| #13434 | [Prompt engineering overview](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/overview) - Anthropic (HTML) | `books/free-programming-books-subjects.md` › Prompt Engineering | The old docs.anthropic.com URL now redirects, so I used the final URL. The title now matches the page ("Anthropic Prompt Engineering Guide" was made up). I left out the Practical Python entry because it's already listed. |
| #13413 | [Robotics, from scratch](https://robotics.biblio.guru) - Kiran Pachhai (HTML) | `books/free-programming-books-subjects.md` › **new Robotics section**, added to the index | Moved from courses to books, as the review said ("this is a book"). |
| #13402 | [ML Academy](https://mltraining.org) - Cagri Temel | `more/free-programming-interactive-tutorials-en.md` › Artificial Intelligence | Moved from courses to interactive tutorials, as the review said. |
| #13384 | [Curso de HTML5 \[40 Horas\]](https://www.cursoemvideo.com/curso/html5/) - Gustavo Guanabara (Curso em Vídeo) | `courses/free-courses-pt_BR.md` › HTML and CSS | Title fixed as the review asked. I moved it from books to courses because it's a video course, and added an account note because a login is required. |
| #13374 | aiOlaOla "Learn AI Coding, from zero" / "Build AI Agents, from zero" (10 entries: en, es, ja, ko, zh) | `courses/free-courses-{en,es,ja,ko,zh}.md` | Fixed the alphabetical-order lint errors. The es/ja/ko titles now match the site (the lesson counts are gone). I added an account-required note in each language because only chapter 1 is open without signing in. |
| #13332 / #13333 | [Introdução a Python com Aplicações de Sistemas Operacionais](https://memoria.ifrn.edu.br/bitstream/handle/1044/2090/EBOOK%20-%20INTRODU%C3%87%C3%83O%20A%20PYTHON%20%28EDITORA%20IFRN%29.pdf) - Fábio Augusto Procópio de Paiva, João Maria Araújo do Nascimento, Rodrigo Siqueira Martins, Givanaldo Rocha de Souza (PDF) | `books/free-programming-books-pt_BR.md` › Python | Title from the review. Full author names taken from the PDF. Parentheses in the URL are encoded. I left out #13333's unrelated change that broke the OpenCV link. |
| #13240 | [LangChain 中文入门教程](https://github.com/liaokongVFX/LangChain-Chinese-Getting-Started-Guide) - liaokongVFX | `books/free-programming-books-zh.md` › 人工智能 | Only this one of the three suggested repos exists. `bytedance/llm-deployment-cookbook` and `ricklamers/llm-developer-handbook-zh` return 404. I left out the CONTRIBUTING-zh changes. |
| #13410 | [JJ_PYTHON_BOOK](https://github.com/joedejesus/JJ_PYTHON_BOOK) - Joe de Jesús Fernández Diniz (GitHub) | `books/free-programming-books-es.md` › Python | The author asked a maintainer to add it because they don't use git. |

### Why is this valuable (or not)?

Each of these was already suggested by someone, and most were accepted except for small changes asked for in review that never got made. Doing those changes here clears out part of the open issue/PR backlog.

### How do we know it's really free?

I opened every link:
- Robotics, from scratch, ML Academy, the IFRN PDF, JJ_PYTHON_BOOK, the LangChain guide and the Anthropic docs can all be read with no account or payment.
- Curso de HTML5 and the aiOlaOla courses cost nothing but need a free account, so they're marked with a note in the list's language (`*(account required)*`, `*(se requiere una cuenta)*`, and so on). Per CONTRIBUTING, course platforms are allowed to require an account.

### For book lists, is it a book? For course lists, is it a course? etc.

Yes. I followed the reviewers' calls on where each one goes: Robotics goes in books, ML Academy in interactive tutorials, and the HTML5 video course in courses.

## Checklist:
- [x] [Search](https://ebookfoundation.github.io/free-programming-books-search/) for duplicates. Checked against the lists. A1Lab, Automate the Boring Stuff, Practical Python and Hacker101 were left out because they're already listed.
- [x] Include author(s) and platform where appropriate.
- [x] Put lists in alphabetical order, correct spacing. `free-programming-books-lint` passes locally on `books/`, `courses/` and `more/`.
- [x] Add needed indications (PDF, access notes, under construction).
- [x] Used an informative name for this pull request.

## Follow-up

- Check the status of GitHub Actions and resolve any reported warnings!

Closes #13410
Supersedes #13434, #13413, #13402, #13384, #13374, #13332, #13333, #13240
