
<h3>//Links</h3>
https://www.youtube.com/watch?v=Uszj_k0DGsg
https://www.udemy.com/course/versionsverwaltung-mit-git-und-github-fur-anfanger/learn/lecture/19451080#overview


von Anbieter  http://git-tower.com
<h3>//CONFIG</h3>
<br><b>Alle Einträge der Konfiguration listen.</b>
<br><i>git config --list</i>
<br><b>Einträge ändern.</b>
<br><i>git config user.name "alias des users"</i>
<br><b>Einträge einzeln ausgeben.</b>
<br><i>git config user.name </i>


 
<h3>//INIT</h3> 
Verzeichnis mit git einrichten
<br><i>git init</i>

<h3>//COMMIT</h3> 
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

<h3>//DIFF</h3>
Was geht ab …oder…kommt hinzu 
git diff <coding des commits/reverts aus dem Log>

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
<h3>//PULL</h3>
<br><i>git pull origin main</i>
<p>Es wird geschaut ob es Änderungen (direkt in Git oder von anderen Usern) 
stattgefunden und merged das mit den lokalen Ressourcen...</p>
<p>wenn das erste mal connected wird muss authentifiziert 
dazu muss unter Einstellungen->Developer ein Token eingerichtet werden...
wenn beim pull eventuelle Histories im Wege sind
</p>
<br><b>Pull der die unterschiedliche Histories lokal und online ignoriert...</b>
<br><i>git pull origin main --allow-unrelated-histories</i>
wieder raus
<h3>//PUSH</h3>
<p>Auch hier wird eine Authentifizierung mit TOKEN vorrausgehen.</p>
<p class="red">Achtung! es werden nur änderungen eingespielt die commited wurden</p>
<br><i>git push origin main</i>
<h3>//FETCH</h3>
<p>
Mit diesem Befehl kann man sich vergewissern, ob es irgendwelche Änderungen
Im Online-Repository gegeben hat.
<br>Wenn das der Fall sollte gepullt werden.
</p>
<h3>//CLONE</h3>
<p>
Wenn man das gesamte Projekt gerne bearbeiten/weiterentwickeln will
zieht man sich einen clone 
</p>
<br>git clone <https://pfad/da/hin>
<h3>GITHHUB-Projekte</h3>
<p>Diese</p>

<h3>GITHUB-Packages</h3>


