# Andrew Masker — CV / Resume

**Robotics resume:** [Download PDF](https://raw.githubusercontent.com/AndrewMasker/CV_Resume_AIM/build/main.pdf) · [View on GitHub](https://github.com/AndrewMasker/CV_Resume_AIM/blob/build/main.pdf)

**Academic CV:** [Download PDF](https://raw.githubusercontent.com/AndrewMasker/CV_Resume_AIM/build/academic.pdf) · [View on GitHub](https://github.com/AndrewMasker/CV_Resume_AIM/blob/build/academic.pdf)

[![CV preview](https://raw.githubusercontent.com/AndrewMasker/CV_Resume_AIM/build/preview.png)](https://github.com/AndrewMasker/CV_Resume_AIM/blob/build/main.pdf)

## Layout

| File | Purpose |
| --- | --- |
| `main.tex` | Robotics / robot learning resume (the one Overleaf compiles) |
| `academic.tex` | Full academic CV |
| `preamble.tex` | Shared packages and page geometry |
| `sections/*.tex` | Sections for the academic CV; `education` and `publications` are shared with the resume |
| `sections/robotics/*.tex` | Sections specific to the robotics resume |
| `CREDITS.md` | Where the LaTeX template came from, and its license |

To add another version, copy `main.tex` or `academic.tex` to a new file,
keep, drop or swap `\input{sections/...}` lines as needed, and add the new
file to `root_file`, the artifact paths, and the publish step in
`.github/workflows/build.yml`. The preview image above shows `main.tex`.

## Builds

Every push to `main` compiles the PDF and force-pushes it, with a preview
image, to the `build` branch, which the links above point to. Pull requests
are compiled too; their PDF can be downloaded from the run's Artifacts.
Build output is kept off `main` so Overleaf's GitHub sync never pulls it in.
