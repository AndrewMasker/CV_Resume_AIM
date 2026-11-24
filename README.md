# Andrew Masker — CV / Resume

**[Download PDF](https://raw.githubusercontent.com/AndrewMasker/CV_Resume_AIM/build/main.pdf)** · [View on GitHub](https://github.com/AndrewMasker/CV_Resume_AIM/blob/build/main.pdf)

[![CV preview](https://raw.githubusercontent.com/AndrewMasker/CV_Resume_AIM/build/preview.png)](https://github.com/AndrewMasker/CV_Resume_AIM/blob/build/main.pdf)

## Layout

| File | Purpose |
| --- | --- |
| `main.tex` | Full CV (root document; the one Overleaf compiles) |
| `preamble.tex` | Shared packages and page geometry |
| `sections/*.tex` | One file per section, shared by every version |

To add another version (e.g. a one-page resume), copy `main.tex` to a new
file, keep or drop `\input{sections/...}` lines as needed, and add the new
file to `root_file` and the publish step in `.github/workflows/build.yml`.

## Builds

Every push to `main` compiles the PDF and force-pushes it, with a preview
image, to the `build` branch, which the links above point to. Pull requests
are compiled too; their PDF can be downloaded from the run's Artifacts.
Build output is kept off `main` so Overleaf's GitHub sync never pulls it in.
