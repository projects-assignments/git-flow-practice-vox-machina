# git flow practice


## Instrucciones
## Primer coder
```sh
git clone <url>
git checkout -b develop
git push origin develop
```
## Todos los coders
```sh
git clone <url>
git switch develop
git checkout -b <rama-con-mi-nombre, por ejemplo: feat-raul>
# realiza cambios en tu rama
git checkout develop
git merge feat-raul
git push origin develop
```
## Último coder
```sh
git switch develop
git pull origin develop
git checkout main
git merge develop
```
## FAQ

**¿ No me deja subir los cambios desde develop ?**

```sh
git pull origin develop
git checkout feat-raul
git rebase develop --continue
git checkout develop
git merge feat-raul
```

