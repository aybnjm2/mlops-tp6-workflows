# Orchestrateur ou integration continue ? (TP06)

| Critere | Prefect (orchestrateur) | GitHub Actions (CI) |
|---|---|---|
| Ce qui declenche l'execution | Planification hebdomadaire ou lancement manuel. | Chaque `git push` ou lancement manuel. |
| Ou s'execute le traitement | Sur une machine locale avec serveur ou worker. | Sur un runner Linux de GitHub. |
| Qui surveille, et ou | Prefect, depuis son interface web. | GitHub, depuis l'onglet Actions. |
| Ce qui se passe en cas d'echec | Le workflow passe à Failed et identifie la tâche en erreur. | Le job passe en rouge et affiche les journaux d'erreur. |
| Type de tache adapte | Planification et exécution des workflows MLOps. | Vérification automatique du code et du pipeline. |
| Ce qui est versionne dans Git | Code Python, paramètres et configuration Prefect. | Fichiers YAML, scripts et dépendances CI. |

## Conclusion (5 lignes)

Prefect permet de planifier et surveiller les workflows MLOps.
GitHub Actions vérifie automatiquement le code à chaque modification.
Prefect gère l'exécution des tâches et leurs erreurs.
GitHub Actions détecte les problèmes avant la mise en production.
Les deux outils sont complémentaires et ne se remplacent pas.