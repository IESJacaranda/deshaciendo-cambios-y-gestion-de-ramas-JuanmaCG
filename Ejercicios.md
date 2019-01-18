1. Tienes que modificar la escena 5 de Hamlet en el fichero scene-5.txt. En dicha escena Hamlet encuentra al fantasma de su padre. Añade este texto al fichero:
> Ghost: 
> My hour is almost come,
> When I to sulphurous and tormenting flames
> Must render up myself.

mkdir examen
Hacer pull/clone del repositorio a la carpeta
nano scene-5.txt y modificas

2. Añade scene-5.txt al área de preparación.

git add scene-5.txt

3. Haz un commit con los cambios con un buen mensaje de commit.

git commit -m "buen mensaje de commit"

4. Modifica las palabras del fantasma. Aquí tienes una sugerencia divertida:
> Ghost: 
> My hour is almost come,
> When I to sulphurous and tormenting balloons
> Must render up myself.

nano scene-5.txt y añades el texto

5. Devuelve el fichero al estado del último commit.

git log --oneline
git reset --mixed f2607c7 

6. Cambia el nombre de LARRY por LAERTES en los ficheros scene-3.txt y scene-7.txt.

nano scene-3.txt
nano scene-7.txt

7. Añade los ficheros al área de preparación usando un único comando git.

git add .

8. Vamos a cometer un error a propósito. Borra cualquier línea del fichero scene-2.txt.

nano scene-2.txt (primera linea)

9. Añade scene-2.txt al área de preparación.

git add scene-2.txt

10. Comprueba el estado del repositorio. 

git status

11. Devuelve scene-2.txt al directorio de trabajo.

git reset scene-2.txt

12. Haz un commit para guardar los cambios realizados en el nombre de Larry por Laertes.

git commit -m "nombres de Larry"

13. Busca el primer commit que has hecho y vuelve a dicho commit. Indica como has buscado el commit anterior y como has vuelto a él.

buscamos el commit con 
git log --oneline
y nos vamos a el:
git reset --hard f2607c7

14. Crea una nueva rama llamada **reinventando_hamlet**

git branch reinventando_hamlet

15. Cámbiate a dicha rama

git checkout reinventando_hamlet

16. Mejora la escena 2 como creas conveniente.

nano scene-2.txt 

17. Haz un commit con los cambios con un mensaje adecuado.

git add scene-2.txt
git commit -m "scene-2 mejorada"

18. Vuelve a la rama master.

git checkout master

19. Elimina la rama **reinventando_halet**

git branch -D reinventando_hamlet 

20. Crea una nueva rama, modifica algo en la rama master, haz commit y llévate los cambios a la rama que has creado.

nano scene-2.txt
git add scene-2.txt
git commit -m "hola"
git checkout nueva
git merge master 

21. Provoca un conflicto entre la rama master y la rama que has creado (indica lo que has hecho). Une la rama a la rama master resolviendo el conflicto.

1- Modificas el fichero scene 2 en la linea 1 (rama master) git add y git commit
2- Modificas el mismo fichero en la misma linea en la rama "nueva" git add y git commit
3- En cualquiera de las ramas haces: git merge "master/nueva" y saltara el conflicto
4- Editas el fichero y borras la linea que quieres eliminar
5- Vuelves a añadir y commit
6- Conflicto resuelto












