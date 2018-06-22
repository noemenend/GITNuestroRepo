
# GITNuestro de cada dia

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRErJhJFIOe5LTdkKcy-ucsVGf8dJo_TiVuKBneClxNfvF08YfdWA)

---

---

1. **¿Qué comando utilizaste en el paso 11?**   
`git reset --hard HEAD~1`  
**¿Por qué?** Porque quiero quedarme con mi working directory exactamente igual que en el commit anterior (padre) que es dónde añadí el archivo inicial sin formato *markdown*.  Si hubiera hecho un *reset 'soft'* mantendría en mi working directory los cambios en el archivo git-nuestro.md.		

2. **¿Qué comando o comandos utilizaste en el paso 12?** **¿Por qué?**  
`git reflog` : Para obtener el **HASH id** del **commit** dónde se añade el estilo.  
`git reset --hard 29d6482` : para recuperar el commit.

3. **El merge del paso 13, ¿Causó algún conflicto?**
No ha causado ningun conflicto.  
**¿Por qué?** Ya que la rama styled que absorbia a master contenia  todos los commits(cambios) y por tanto no habia ninguna diferencia entre ambos.

4. **El merge del paso 19, ¿Causó algún conflicto?**
Sí en este caso hubo conflicto.  
**¿Por qué?** Porque que archivo git-nuestro.md fue modificado tanto en la rama htmlfy como en la rama styled.

5. **El merge del paso 21, ¿Causó algún conflicto?**
No ha causado ningun conflicto.  
**¿Por qué?** Porque styled contenia los *commits* de master

6. **¿Que comando o comandos utilizaste en el paso 25?**  
`git graph`, porque previamente creé ese alias para evitar teclear el comando completo: `git log --graph --decorate --pretty=oneline`  

7. **El merge del paso 26, ¿Podría ser fast forward?** 
Si podría ser fast forward.  
**¿Por qué?** Porque la rama title contiene todos los commits de la rama master.
  De hecho si no lo forzamos por defecto seria fast forward.
  
8. **¿Que comando o comandos utilizaste en el paso 27?**  
`git reflog` : Para obtener el commit anterior  
`git reset HEAD1` : Para irnos al commit anterior y no perder los cambios hechos en el archivo git-nuestro.md.

9. **¿Que comando o comandos utilizaste en el paso 28?**  
`git checkout -- git-nuestro.md`: Descartamos los cambios  
`git status` : Vemos que ahora en nuestro working directory no hay cambios que subir al staging

10. **¿Que comando o comandos utilizaste en el paso 29?**  
`git branch -D title`

11. **¿Que comando o comandos utilizaste en el paso 30?**  
`git reflog` : Para saber cual es el commit al que queremos ir  
`git reset --hard 1470387`: Para situarnos en el merge que acabamos de hacer

12. **¿Que comando o comandos utilizaste en el paso 32?**  
`git reflog` : Para ver el hash id del commit inicial  
`git reset --hard 3264c7c`  
HEAD is now at 3264c7c Añado el archivo git-nuestro.md: Commit inicial

13. **¿Que comando o comandos utilizaste en el paso 33?**  
`git reflog`: Obtengo el hash id del commit en el que se añadió el título  
`git reset --hard 5251cba`  
HEAD is now at 5251cba Añadiendo titulo a git-nuestro.md  

---


