---


---

<p>En la siguiente imagen se muestra la subrutina que consume más CPU, la cual es levenshtein, este reporte fue generado por kcachegrind por medio de callgrind.<br>
<img src="https://lh3.googleusercontent.com/djNlRY-69DEPIwKBz_9EVymb7q_6ei8ms-4blIsyM7Th5G0cjMZBkC0gxo1w67XRN1mhx-MV-X3d" alt="" title="la subrutina que consume más cpu"></p>
<p>Se muestra el árbol de llamados a esa subrutina.<br>
<img src="https://lh3.googleusercontent.com/ecXHWrWsAYEnG2zWWRUFa6X4xvq8Ii7JeTh8ArnVDSsTKEmLU03TE1sN-qwi1rv8mUpTMHqEo_Je" alt="" title="Arbol de llamados a la función levenshtein"></p>
<p>Ahora para medir el tiempo que toma el programa se utilizó la herramienta gprof. se compara el tiempo dado por el programa y el tiempo dado por gprof.</p>
<p>Imagen del tiempo dado por el programa.<br>
<img src="https://lh3.googleusercontent.com/LOyf4sXiJv8rDnEcz-8qaix55wa7ZxF0jgrVadKMcVIzCCWbWbHLQWFhjGOWpIE2ZqhbzE6eFExw" alt="" title="tiempo programa"></p>
<p>Imagen de tiempo dado por gprof.<br>
<img src="https://lh3.googleusercontent.com/QGugdB0CXoI02YVqsmt1hFjAoSocyRFjga78zoPIVV9eH9xUspdVDfMmTxOJ6ErmB5wWTljuIv7K" alt="" title="gprof"></p>
<p>Se puede observar que el tiempo dado por el programa de solamente lo que duran las comparaciones, es decir, la función levenshtein es de 2364 y el tiempo dado por gprof de solo esta subrutina es de 2361 lo que nos lleva a la conclusión de que al ser una diferencia mínima de 3 segundos los tiempos son similares y coinciden los resultados. También se afirma que los resultados de gprof nos muestran que los  obtenidos de callgrind son correctos, ya que la subrutina que consume más tiempo es levenshtein por lo tanto tambien consume más CPU.</p>

