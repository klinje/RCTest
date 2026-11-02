# branch erstellen und mergen

- Als erstes habe ich den branch erstellt mit `git branch <name>` und dann bin ich in den branch gewechselt mit `git switch <name>`
- Anscheinend kann man aber auch direkt `git switch -c <name>` benutzen, um einen branch zu erstellen und direkt dahin zu switchen (`-c` ist die `create option`)

## Gotchas

- bevor ich `git push` nutzen konnte musste ich erstmal `git push --set-upstream origin <name>` benutzen, damit git überhaupt weiß, wohin der branch gepusht werden soll. Es wird sozusagen der lokale branch mit dem remote branch verknüpft.
    - es können wohl auch unterschiedliche namen für lokale und remote branches vergeben werden
    - dafür müsste man `git push -u origin <local_name>:<remote_name>` nutzen
