#hello commit

######What are the benefits of commits?
Git Commits bieten eine detaillierte Versionshistorie, die die Verfolgung des Codes,
die Zusammenarbeit und die Fehlerbehebung erleichtert. Sie ermöglichen eine genaue
Überprüfung des Codes und die Möglichkeit, Änderungen bei Bedarf rückgängig zu machen.
Commit-Nachrichten dokumentieren Änderungen und bieten Kontext und Verantwortlichkeit
für Code-Änderungen.

######Is there another way to verify a commit was created?
Ja, man kann mit git log schauen, ob sich etwas änderte. Auch gibt es "git show (hash vom commit)'', damit kann man auch sehen, was sich änderte.

######How to check if a file is tracked and if not, then track it?
Mit "git ls-files --error-unmatch <Ort vom File>" kann man schauen ob etwas von Git getracked ist oder nicht.
Wenn man es eingibt, wird gesagt, wie die Datei heisst. Wenn es nicht getracked wird, 
wird einfach nichts gesagt. 

Um die Datei dann zu tracken, falls es noch nicht getracked ist, muss man mit "git add <Ort vom File>"
die Datei für die nächsten Änderungen / commits vorbereiten. Nachdem man das gemacht hatte, macht man
einfach "git commit -m "Tracking <Dateiname>".

- test
- test
- test

######In which situation should you use 'git diff'?
Du solltest 'git diff' benutzen, um die Unterschiede zwischen verschiedenen Zuständen deines Git Repositorys zu vergleichen,
einschließlich nicht committeter Änderungen, Commits, Branches und Dateien. Dies hilft dir, Unterschiede zu verstehen und
Änderungen zu überprüfen, bevor du Commits erstellst oder Änderungen zusammenführst.
 
######How do you create a patch with `git diff`?
Mit dem Befehl git diff kannst du einen Patch erstellen, der die Unterschiede zwischen zwei Commits oder zwischen deinem Arbeitsverzeichnis und dem letzten Commit darstellt.