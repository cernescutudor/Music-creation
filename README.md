## Mod de lucru Git/GitHub + comenzi pentru consola (Git Bash):
- cloneaza proiectul de pe GitHub (*git clone https://github.com/912-Cseke-Stefan/Music-creation*)
- pentru a lucra, creeaza un branch local (*git branch <name>*) si schimba branch-ul curent pe cel 
         tocmai creat (*git checkout <name>*)
- fisierele modificate trebuie sa fie marcate pentru commit (*git add .* -> in folderul principal; 
         in GUI, actiunea ar trebui sa apara sub numele de 'Stage changes'), dupa care se face 
         commit-ul (*git commit -m "message"*)
- pentru a da merge in branch-ul main, schimbi pe branch-ul main (*git checkout main*), actualizezi 
         branch-ul main la versiunea sa din proiectul de pe GitHub (*git pull*; aceasta face 
         implicit *'git pull origin main'*, care da merge la branch-ul main de pe online la 
         branch-ul local curent, adica main), dupa care dai merge la branch-ul de lucru in 
         branch-ul curent (*git merge <name>*)
    De notat: daca lucrezi local tot pe main, *git pull* s-ar putea sa aiba conflicte; daca lucrezi
            pe branch separat, conflictele o sa apara la *git merge*. Consider ca e mai ok asa, 
            desi oricum e foarte indicat sa lucrati cu branch-uri si sa le denumiti sugestiv, in 
            functie de ce vreti sa faceti la momentul respectiv, deoarece alea raman in istoric 
            pe remote.
- daca apar conflicte, am pus un link care arata cum se rezolva, Visual Studio are de asemenea 
         GUI pentru rezolvarea lor, dar, in orice caz, ne putem auzi sa vedem cum se rezolva
- dupa ce branch-ul main local a fost actualizat, modifica branch-ul main de pe GitHub 
         (*git push origin main*); nu am configurat sa fie nevoie de pull request, deci ar trebui 
         sa ruleze fara probleme si modificarile sa fie vizibile imediat pe GitHub

O clarificare suplimentara, fiecare o sa se raporteze la doua repouri: cel remote si unul propriu 
local. O sa lucram cu un branch pe remote, si anume main; restul branch-urilor cu care o sa avem 
de-a face o sa fie proprii si locale pentru fiecare dintre noi. Acesta ar fi cel mai simplu mod 
de lucru dupa parerea mea.

## FAQ:
Ce e origin?
'origin' e numele repository-ului online pe care l-ai clonat.

### Niste tutoriale bune:
https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes
https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell
https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging