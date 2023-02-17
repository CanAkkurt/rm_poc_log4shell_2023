# Samenvattting - Opzetten werkomgeving

## Basisoftware via Choco

```bash
choco install -y git        # CLI client
choco install -y gitkraken  # Grafische Git client (optioneel)
choco install -y miktex     # LaTeX distributie
choco install -y texlive    # Alternatieve LaTeX distro (kies 1 van de 2!)
choco install -y texstudio  # Complete LaTeX IDE
choco install -y vscode     # Visual Studio Code (optioneel)
choco install -y JabRef     # Bibliografische databank
choco install -y typora     # Markdown editor (optioneel)
```

## Configuraties

### Fonts

- [Montserrat Regular, ExtraBold](https://fonts.google.com/specimen/Montserrat)
- [Code Pro Black](https://www.dafontfree.net/freefonts-code-pro-black-f62435.htm)
- Fira Code: `choco install firacode`

### Git, Github

[sleutelpaar aanmaken](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

```bash
git config --global user.name "Pieter Stevens"
git config --global user.email pieter.stevens.u12345@student.hogent.be
git config --global github.user PieterStevens

git config --global push.default simple
git config --global pull.rebase true
git config --global rebase.autoStash true
git config --global init.defaultBranch main
```

#### ConfigFile `.gitconfig`

```gitconfig
[user]
    name = Thomas Thomas
    email = thomas.thomas.y3313@student.hogent.be
[push]
    default = simple
[pull]
    rebase = true
[core]
    autocrlf = input
```

#### Workflow (meerdere personen)

1. Zorg eerst dat je alle lokale wijzigingen gecommit zijn: `git status`
2. Haal de wijzigingen van de andere teamleden van Github: `git pull --rebase`
3. Stuur tenslotte je wijzigingen naar Github: `git push`

| Command                   | Uitleg                                             |
| :------------------------ | :------------------------------------------------- |
| `git status`              | Status van huidige project                         |
| `git add FILE...`         | Selectie van bestanden voor de commit (indexeren)  |
| `git commit -m 'MESSAGE'` | Commit wijzigingen naar de lokale repostory        |
| `git push`                | Push lokale wijzigingen naar de remote repository  |
| `git pull`                | Pull wijzigingen van remote naar lokale repository |

### LaTeX

```txt
Build:
 - Default Compiler: XeLaTeX
 - Default Bibliography tool: biber

Commands:
 - XeLaTeX: xelatex -synctex=1 -interaction=nonstopmode -shell-escape %.tex

Editor:
 - Indentation mode: Indent and Unindent Automatically
 - Replace Indentation Tab by Spaces: Aanvinken
 - Replace Tab in Text by spaces: Aanvinken
 - Replace Double Quotes: English Quotes: ``''
```

#### Aanmaken pdf-bestand

- pdf compileren: `Tools > Build & View` (F5)
- bibliografie toevoegen: `Tools > Bibliography` (F8)

#### Alternatief VSCode

choco install -y texlive (in plaats van MikTEX)
choco install -y vscode

Extensies:

- LATEX Workshop (James Yu)
- GitLens (GitKraken)
