# Práctica 1: Suma de 5 números
## 1. Descripción del problema (Fase 1)
El programa pide 5 numeros uno por uno y los va sumando y nal final muestra el resultado final

_____

## 2. Entradas y salidas (Fase 1)
<!-- Define cada entrada y cada salida, con su tipo de dato y su objetivo. -->

**Entradas:**
1. Cinco numeros

**Salidas:**
1. La suma total de los numeros

## 3. Restricciones e invariante (Fase 1 y 2)

**Restricciones** (¿qué debe cumplirse?):
- exactamente 5 numeros
- la contidad no cambia durante la ejecucion

**Decisión sobre negativos y decimales** (¿los acepto? ¿por qué?):
si, porque utilizo double

**Invariante** (¿qué es verdad después de cada vuelta del ciclo?):
la suma de los numeros leidos hasta el momento

## 4. Casos resueltos a mano (Fase 1)

| Caso | Números | Suma calculada a mano |
|---|---|---|
| 1 | 1, 2, 3, 4, 5 | 15 |
| 2 | -3, 5, -2, 10, -1 | 9 |
| 3 | 1, 2, 3, 4, V | No se puede calcular |

## 5. Receta en pseudocódigo (Fase 2)
<!-- Tu receta va en el archivo RECETA.md. Aquí solo responde las dos preguntas. -->

**¿Probé mi receta a mano con un caso?** Sí 
**¿Tuve que corregirla?** No

## 6. Cómo compilar y ejecutar (Fase 3)

```bash
g++ -Wall -Wextra -std=c++17 main.cpp -o suma
./suma
```

## 7. Ejemplo de ejecución (Fase 3)
 ./suma
Suma de 5 numeros
Numero 1 de 5: 1
Numero 2 de 5: 2
Numero 3 de 5: 3
Numero 4 de 5: 4
Numero 5 de 5: 5
Total: 15

## 8. Experimentos (Fase 3)

**Experimento A: ¿qué pasó al no inicializar `suma`?**
No me ninguna advertencia

**Experimento B (opcional): ¿qué pasó al usar `int` con 2.5?**
al usar int y poner 2.5 el programa solo guardo el 2 y se salto los demas numeros sin dejarme escribirlos

## 9. Tabla de pruebas (Fase 4)

| Caso | Números | Esperado | Obtenido | ¿Pasó? |
|---|---|---|---|---|
| Del 1 al 5 | 1 a 5 | 15 | 15 | si |
| Todos ceros | 0 ×5 | 0 | 0 | si |
| Con negativos | -3, 5, -2, 10, -1 | 9 | 9 | si |
| Decimales | 0.5 ×5 | 2.5 | 2.5 | si |
| Todos iguales | 7 ×5 | 35 | 35 | si |
| Caso propio 1 | 100, 200, 300, 400, 500 | 1500 | 1500 | si |
| Caso propio 2 | 1.5, -2.5, 3, 0, 4 | 6 | 6 | si |

## 10. Bitácora de mejoras (Fase 4)

| # | ¿Qué falló o qué quise mejorar? | ¿Qué cambié? | ¿Funcionó? |
|---|---|---|---|
| 1 | los mensajes salian pegados ("Numero1de5")| agrege espacios dentro de las comillas| si |


**Reto elegido (opcional):** ninguno

## 11. Dudas para el profesor (Fase 3)

| Duda | Lo que ya intenté |
|---|---|
| ¿como hago que el programavuelva a perir un numero si es invalido como V?

## 12. Reflexión final

**¿Qué aprendí con esta práctica?**
la diferencia entre int y double

**Ahora que terminé, ¿qué cambiaría de mi proceso?**
haria commits desde el principio

**¿Qué fue lo más difícil y cómo lo resolví?**
Lo más difícil fue entender cómo funciona el ciclo for y el contador. Lo resolví comparándolo con mi receta en pseudocódigo y siguiendo a mano cómo cambiaban suma y contador en cada vuelta.

**¿Qué pregunta me quedó sin responder?**
ninguna

## 13. Lista de verificación antes de entregar (Fase 5)

- [ si ] Llené todas las secciones (no quedan `_____`)
- [ si ] Mi programa compila sin advertencias
- [ si ] Probé todos los casos de la tabla
- [ si ] Hice al menos 3 commits con mensajes claros
- [ si ] Hice `git push` y verifiqué mi fork en GitHub
- [ si ] Entregué el enlace de mi fork en Classroom