<h3>General</h3>
https://www.youtube.com/watch?v=Uszj_k0DGsg
https://www.udemy.com/course/versionsverwaltung-mit-git-und-github-fur-anfanger/learn/lecture/19451080#overview


von Anbieter  http://git-tower.com

commit…
git commit <file>
Achtung beim commit öffnet sich der VI-Editor (esc-taste drücke und dann :wq eingeben)
git commit  -m „das habe ich getan“ <file>

<h3>//LOG</h3> 
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

<h3>//BRANCH</h3>
Anlegen von branches bzw. forks
git branch  <name>

In einen branch wechseln
git checkout <name>
  
<h3>//STASH</h3>
um Zwischenstände zu speichern bzw. Alternativen auszuprobieren
dem stash muss ein commit der Datei(en) vorangegangen sein.
git stash save <name> 
Vorzugsvariante reaktivieren
<ul><li>git stash list
<br>stash@{1} ….
<br>stash@{2} ….
  </li>
  <li>git stash apply stash@{2}</li>
  <li>git stash clear (löschen des Stashs)</li></ul>

//MERGE
man bereinigt die Datei… und macht ein commit …
Danach läßt man sich mit git status den aktuellen Status ausgeben.
Wenn alles 0kay ist kann es weiter gehen.

vereinbaren von regeln/Konv. für die Arbeit mit Repos.
<h3>//GITHUB FLOW</h3>
<i>git remote add origin htts://path/to/repository</i>
<br>erstmal ist damit die quelle des Online-Repositories
genannt 
<br><b>entfernen der Kopplung des Repository's</b>
<br><i>git remote remove origin </i>
<br><b>Holen der der Resourcen aus dem Repository</b>
<br><i>git pull origin main</i>

wenn das erste mal connected wird muss authentifiziert 

GITFLOW

