## Reporte

Despues de compilar profile_me_1.c con el siguiente comando:
```
gcc profile_me_1.c  -pg -o program.e

```

Intento ejecutar program.e, pero no me deja me salta segmentation fault. Luego antes de ejecutar el programa nuevamente pongo lo siguiente:
```
ulimit -s unlimited

```
Ahora ya si puedo ejecutarlo normalmente y me genera el archivo gmon.out. Luego ejecuto gprof mostrandome un resumen del tiempo gastado por el programa y cada una de sus funciones
```
gprof program.e gmon.out

```
Luego aplico una optimizacion mas agresiva, compilando nuevamente con el siguiente comando
```
gcc profile_me_1.c  -pg -o03 program.e

```
Despues de este ultimo paso vuelvo a ejecutar y correr  gprof y el tiempo de ejecucion disminuyo un poco




