# Día 1: Git Avanzado

En este día aprenderás comandos avanzados de Git.

## Contenido
- Rebase vs Merge
- Cherry-pick
- Stash
- Reset y revert

## Tareas

### Tarea 1: Git Stash
Practica guardando cambios temporalmente:
```bash
git stash           # guardar cambios
git stash list      # ver stashes
git stash pop       # recuperar último
git stash apply     # aplicar sin eliminar
git stash drop      # eliminar stash
```

### Tarea 2: Cherry-pick
Aplica commits específicos:
```bash
git cherry-pick <commit-hash>
```
Usa cuando necesites un commit de otra rama.

### Tarea 3: Reset y Revert
Entiende la diferencia:
```bash
git reset --soft HEAD~1   # mantiene cambios staged
git reset --mixed HEAD~1  # mantiene cambios unstaged
git reset --hard HEAD~1   # elimina cambios
git revert <commit>       # crea commit inverso
```

## Ejercicios Adicionales
- Practica con rebase interactivo
- Experimenta con git reflog
