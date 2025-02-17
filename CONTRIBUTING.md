# Cosas en las que puedes ayudarnos
* Referencias que se nos hayan pasado apuntar de lo que hablamos en los capítulos
* Apuntes sobre cosas que son incorrectas o inexactas
* Correcciones ortográficas

# Pasos a seguir
1. Haz fork del repo en tu cuenta
2. Lanza 
```
git submodule update --init --recursive
```
3. Lanza en local el blog de Hugo:
```
hugo server --disableFastRender --buildFuture --buildDrafts --cleanDestinationDir
```
4. Haz las modificaciones
5. Crea una Pull Request (PR)
