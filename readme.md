
<h3>//Links</h3>
<br>
https://www.youtube.com/watch?v=Uszj_k0DGsg
<br><i>allgemeines Video</i>
<br>
https://www.udemy.com/course/versionsverwaltung-mit-git-und-github-fur-anfanger/learn/lecture/19451080#overview
<i>Kurs bei Udemy  - kostenpflichtig</i>
<br>https://pages.cms.hu-berlin.de/cms-webtech/gitlab-documentation/docs/git-befehle/

<br><i>Beschreibung der wichtigsten Befehle von der HU-Berlin</i>
<br><i>Erklärung zum Anlegen eines neuen Projektes auf GITHUB mit allen optionalen Einstellungen</i>
<br><i>Erklärung zum Anlegen eines neuen Projektes auf GITHUB mit allen optionalen Einstellungen</i>

<h3>//Software die Arbeit abnimmt</h3>
http://git-tower.com
<h3>//Online Repositories  - Plattformen</h3>
<br>http://github.com
<br>http://bitbucket.com
<br>http://gitlab.com

wq
<h3>//CONFIG</h3>
<p>Git ermöglicht lokale und globale (mit command --global) Einstellungen</p>
<br><b>Alle Einträge der Konfiguration listen.</b>
<br><i>git config [--global] --list</i>
<br><b>Einträge ändern.</b>
<br><i>git config [--global] user.name "alias des users"</i>
<br><b>Einträge einzeln ausgeben.</b>
<br><i>git config [--global] user.name </i>


 
<h3>//INIT</h3> 
Verzeichnis mit git einrichten
<br><i>git init</i>

<h3>//COMMIT</h3> 
<b>Einzelne Datei "commiten" </b>
<br><i>git commit -m "text zu commit" <file></i>
<br><b>Ganzes Verzeichnis bzw. alle Dateien commiten</b>
<br><i>git commit -m "text zu commit" --all</i>
<br><b>Datei oder Verzeichnis  "commiten" ...</b>
<br><i>git commit <file|--all></i>
<p style="color:red;">
Achtung beim commit öffnet sich der VI-Editor (esc-taste drücke und dann :wq eingeben)
</p>

<h3>//LOG</h3> 
<b>Änderungen anzeigen (mit der option -s in verkürzter  Form)</b>
<br><i>git show -s</i>
<br><b>bessere verkürzte/ganz kurze  Darstellung</b>
<br><i>git log —oneline</i>
<br><b>einzeilige Darstellung der Änderungen  (mit grafischem Baum)</b>
<br><i>git log --graph --online</i>

<h3>//DIFF</h3>
Was geht ab …oder…kommt hinzu 
git diff <coding des commits/reverts aus dem Log>

Alten Zustand einer Datei wiederherstellen 
git revert <code des commits/reverts aus dem Log>

<h3>//BRANCH</h3>
<p>
Je nachdem wie man sein Projekt entwickelt gibt es unterschiedliche Philosophien
/Absprachen zwischen Entwicklern wie ins git commitet wird.
Angelegt werden verschiedene Branches und Sub-branches.
</p>
<b>Anlegen eines Branches</b>
<br><i>git branch [name]</i>
<br><b>Anlegen eines Branches und sofort in den Branch wechseln</b>
<br><i>git branch -a [name]</i>
<br><b>In einen Branch wechseln</b>
<br><i>git checkout [name] </i> 

<h3>//STASH</h3>
<p>
Um Zwischenstände zu speichern bzw. Alternativen auszuprobieren
dem stash muss ein commit der Datei(en) vorangegangen sein.
</p>
<b>Speichern einer Version im stash</b>
<br><i>git stash save [Name der Datei]</i>
 
Vorzugsvariante reaktivieren
<ul><li>git stash list
<br>stash@{1} ….
<br>stash@{2} ….
  </li>
  <li>git stash apply stash@{2}</li>
  <li>git stash clear (löschen des Stashs)</li></ul>

<h3>//MERGE</h3>
man bereinigt die Datei… und macht ein commit …
Danach läßt man sich mit git status den aktuellen Status ausgeben.
Wenn alles okay ist kann es weiter gehen.

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


