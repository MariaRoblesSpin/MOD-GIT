# Práctica del curso de git, github y Sourcetree

- **¿Qué comando utilizaste en el paso 11? ¿Por qué?**
El comando `git reset --hard HEAD~1` para perder los cambios del working copy.

- **¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**
El comando `git reflog` para localizar el código del commit que quería recuperar (`985e474`) y `git reset --hard 985e474` para volver a dicho commit. 

- **El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**
No. Porque en realidad no había ningún cambio nuevo en master y todo lo que había en master ya lo contenía la rama styled.

- **El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**
Sí. Porque el contenido del archivo git-nuestro.md en la rama styled era diferente al contenido del mismo archivo en la rama htmlify. 

- **El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**
No. Porque styled se creo desde master y era la evolución desde el contenido de master. Luego el merge ha sido fast forward, sin conflictos y sin commit.

- **¿Qué comando o comandos utilizaste en el paso 25?**

`git log --graph --decorate --pretty=oneline`

- **El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**
Sí. Porque title se ha creado desde master y en master no ha habido cambios luego no puede haber conflicto. He desecho el merge con `git reset --hard` para comprobar mi teoría y por un momento he estado perdida porque no veía el commit del título añadido. Luego me he dado cuenta con el reflog que ese log estaba en la rama title y ya he podido repetir el merge sin en comando --no-ff. Ahora voy a volver a hacerlo con --no-ff y voy a seguir el flujo para deshacerlo sin --hard.

- **¿Qué comando o comandos utilizaste en el paso 27?**
`git reset HEAD~1`

- **¿Qué comando o comandos utilizaste en el paso 28?**
`git checkout -- git-nuestro.md`

- **¿Qué comando o comandos utilizaste en el paso 29?**
`git branch -D title`

- **¿Qué comando o comandos utilizaste en el paso 30?**
`git reflog` para ver los commits.
`git reset --hard 0a098ba` siendo `0a098ba` el código del log del merge que quería recuperar.
- **¿Qué comando o comandos utilizaste en el paso 32?**
`git reset --hard fb65dce` siendo `fb65dce` el código del commit de inicio.
- **¿Qué comando o comandos utilizaste en el paso 33?**
`git reset --hard 0a098ba` siendo `0a098ba` el código del log del merge con el título.





