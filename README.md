## Vilniaus universiteto skaidrių LaTeX šablonas

Sukurtas iš dalies pagal https://github.com/linas-p/VU-MIF-II-slides-template-1.

Šablonas naudoja:  
- `latexmk` kompiliavimo paleidimui  
- `lualatex` PDF generavimui  

## Pasiruošimas

### Linux

Instaliuoti Tex Live.

#### Ubuntu

Užtenka įvydyti `make ubuntu` šio projekto direktorijoje.

### Overleaf

Reikia pakeisti kompiliatorių į LuaLaTeX, žr.: https://www.overleaf.com/learn/how-to/Changing_compiler.

### Windows

Instaliuoti vieną iš:  
- [Tex Live](https://tug.org/texlive/windows.html)  
- [MikTex](https://miktex.org/download), jam reikia papildomai įrašyti `biber`

### macOS

Instaliuoti [MacTex](https://tug.org/mactex).

## PDF generavimas

### Linux / macOS

Įvykdyti vieną iš:  
- `make`  
- `make pdf`  
- `latexmk --lualatex pristatymas.tex`

### Windows

Įvykdyti `latexmk --lualatex pristatymas.tex`.

## Kitos naudingos komandos

### Linux / macOS

- nuolatinis perkompiliavimas dokumentui pasikeitus: `make watch`
- paprastų klaidų patikrinimas (pastaba: praneša apie daugybę dalykų, iš kurių nebūtinai visi aktualūs): `make check`  
- nereikalingų failų išvalymas: `make clean`
