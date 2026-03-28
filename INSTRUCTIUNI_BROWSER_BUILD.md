# Cum scoti EXE-ul fara Visual Studio

Acest pachet contine fisierele modificate pentru 2560x1440 si un workflow GitHub Actions care face build-ul in cloud.

## Ce faci

1. Fa un fork la repo-ul original `clauadv/job_helper` pe contul tau GitHub.
2. In fork, inlocuieste fisierele:
   - `fish/src/dllmain.cpp`
   - `shared/src/pixel/pixel.hpp`
3. Adauga fisierul:
   - `.github/workflows/build-fish-2560x1440.yml`
4. In GitHub, intra la tab-ul **Actions**.
5. Ruleaza workflow-ul **Build fish 2560x1440**.
6. Dupa ce termina, intra in job si descarca artifact-ul `fish-2560x1440-build`.
7. In arhiva rezultata vei avea executabilul din `release/fish/`.

## Observatii

- Proiectul este o solutie Visual Studio/MSBuild pe Windows, nu un proiect simplu de VS Code.
- Configuratia din repo este `release|x64`.
- Daca GitHub iti cere permisiune pentru Actions in fork, apasa Enable Actions.
