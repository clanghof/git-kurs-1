
General
https://www.youtube.com/watch?v=Uszj_k0DGsg
https://www.udemy.com/course/versionsverwaltung-mit-git-und-github-fur-anfanger/learn/lecture/19451080#overview


von Anbieter  http://git-tower.com

commit…
git commit <file>
Achtung beim commit öffnet sich der VI-Editor (esc-taste drücke und dann :wq eingeben)
git commit  -m „das habe ich getan“ <file>

//LOG 
Änderungen anzeigen
git show 
mit der option s 
bzw. 
git log —oneline (bessere verkürzte Darstellung) 
einzeilige Darstellung der Änderungen
git log --graph --online (mit grafischem Baum)

//DIFF
Was geht ab …oder…kommt hinzu 
git diff <code des commits/reverts aus dem Log>

Alten Zustand einer Datei wiederherstellen 
git revert <code des commits/reverts aus dem Log>

//BRANCH
Anlegen von branches bzw. forks
git branch  <name>

In einen branch wechseln
git checkout <name> 
//STASH
um Zwischenstände zu speichern bzw. Alternativen auszuprobieren
dem stash muss ein commit der Datei(en) vorangegangen sein.
git stash save <name> 
Vorzugsvariante reaktivieren
a) git stash list
stash@{1} ….
stash@{2} ….
b) git stash apply stash@{2}
c) git stash clear (löschen des Stashs)

//MERGE
man bereinigt die Datei… und macht ein commit …
Danach läßt man sich mit git status den aktuellen Status ausgeben.
Wenn alles 0kay ist kann es weiter gehen.

vereinbaren von regeln/Konv. für die Arbeit mit Repos.
GITHUB FLOW
GITFLOW

