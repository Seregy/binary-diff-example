# Binary files comparison examples

Comparing binary files with Git by converting them into plain text.

### Set up

Use the command in the `.gitconfig` to include the file into the Git settings.
Check the tools needed for converting the files in the `.gitconfig`.

### Commands

#### Diff

```
git diff config.xlsx

git diff report.docx
```

#### Difftool

```
git difftool --tool opendiff report.docx

git difftool --tool intellij config.xlsx
```

#### Difftool with conversion

```
git difftool --tool pandoc report.docx

git difftool --tool csvkit config.xlsx

git difftool --tool intellij-csvkit config.xlsx
```