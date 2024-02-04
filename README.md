# Compact Awesome CV

**Compact Awesome CV** is LaTeX template for a **CV (Curriculum Vitae)**, **Résumé** or **Cover Letter** inspired by [Awesome CV](https://www.overleaf.com/latex/templates/awesome-cv/dfnvtnhzhhbm). The template reduces spaces between section entries and changes font styles, colors and changing some default icons used in the header.

## Preview

### Résumé

You can see PDF preview of the compact resume layout  [here](https://github.com/capac/Compact-Awesome-CV/blob/main/examples/resume.pdf).

| Page 1 | Page 2 |
|:------:|:------:|
| [![Résumé (First page)](https://github.com/capac/Compact-Awesome-CV/blob/main/examples/resume-0.png)](https://github.com/capac/Compact-Awesome-CV/blob/main/examples/resume.pdf) | [![Résumé (Second page)](https://github.com/capac/Compact-Awesome-CV/blob/main/examples/resume-1.png)](https://github.com/capac/Compact-Awesome-CV/blob/main/examples/resume.pdf) |

### Cover Letter

You can see PDF preview of the compact cover letter layout (without sections) [here](https://github.com/capac/Compact-Awesome-CV/blob/main/examples/coverletter.pdf).

| Without Sections | With Sections |
|:---:|:---:|
| [![Cover Letter (Traditional)](https://github.com/capac/Compact-Awesome-CV/blob/main/examples/coverletter-0.png)](https://github.com/capac/Compact-Awesome-CV/blob/main/examples/coverletter.pdf) | [![Cover Letter (Wth photo)](https://github.com/capac/Compact-Awesome-CV/blob/main/examples/coverletter-1.png)](https://github.com/capac/Compact-Awesome-CV/blob/main/examples/coverletter.pdf) |


## How to Use

### Requirements

A full TeX distribution is required to compile TeX documents. Various distributions for [different operating systems (Windows, Mac, \*nix)](http://tex.stackexchange.com/q/55437) are available, but the recommendation is to install directly from [TeX Live](https://tug.org/texlive/).

#### Linux

On Linux you can [install TeX from upstream](https://tex.stackexchange.com/q/1092) which is recommended because it return the most up-to-date version of TeX Live. You can also run `sudo apt-get install texlive-full` but it's generally not the most up-to-date version.

#### macOS

On macOS you can easily install Tex Live by installing [MacTeX distribution](https://tug.org/mactex/) or, if you have [Homebrew](https://brew.sh), by running `brew install texlive`, which will install the full version, or `brew install basictex` for a minimal TeX working environment.

If you don't want to install the dependencies on your system, this can also be obtained via [Docker](https://docker.com).

### Usage

At a command prompt, run:

```bash
xelatex {your-cv}.tex
```

Or using docker:

```bash
docker run --rm --user $(id -u):$(id -g) -i -w "/doc" -v "$PWD":/doc thomasweise/texlive make
```

In either case, this should result in the creation of ``{your-cv}.pdf``


## Credits

[**LaTeX**](https://www.latex-project.org) is a fantastic typesetting program that a lot of people use these days, especially the math and computer science people in academia.

[**LaTeX FontAwesome**](https://github.com/furl/latex-fontawesome) is bindings for FontAwesome icons to be used in XeLaTeX.

[**Roboto**](https://github.com/google/roboto) is the default font on Android and ChromeOS, and the recommended font for Google’s visual language, Material Design.

[**Source Sans Pro**](https://github.com/adobe-fonts/source-sans-pro) is a set of OpenType fonts that have been designed to work well in user interface (UI) environments.

## Extra resources

[**Fontawesome5 package** document (PDF)](http://mirrors.ibiblio.org/CTAN/fonts/fontawesome5/doc/fontawesome5.pdf) for custom Fontawesome icons in TeX by [Marcel Krüger](https://tex.stackexchange.com/users/80496/marcel-kr%C3%BCger).
