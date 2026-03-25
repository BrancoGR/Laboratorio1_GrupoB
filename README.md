# Laboratorio 1: Simulación de Robot Móvil Diferencial en Webots

## 📌 Descripción

Este laboratorio tiene como objetivo comprender el comportamiento cinemático de un robot móvil diferencial mediante simulación en Webots.

Un robot diferencial utiliza dos ruedas motrices independientes (izquierda y derecha), y su movimiento depende directamente de la velocidad de cada una.

Se implementó un controlador en Python para manipular las velocidades de las ruedas y analizar distintos tipos de movimiento.

---

## Tecnologías utilizadas

- Webots
- Python

---

## Cómo ejecutar la simulación

1. Abrir Webots.
2. Cargar el mundo que contiene el robot diferencial (por ejemplo, e-puck).
3. Abrir el controlador del robot.
4. Ejecutar la simulación.
5. Observar el comportamiento del robot según las velocidades configuradas.

---

## Modelo cinemático

El comportamiento del robot se basa en:

- Velocidad lineal:
  
  v = (vr + vl) / 2

- Velocidad angular:

  ω = (vr - vl) / L

Donde:
- `vr`: velocidad rueda derecha
- `vl`: velocidad rueda izquierda
- `L`: distancia entre ruedas

---

## Experimentos realizados

Se probaron los siguientes casos:

### 1. Movimiento recto
- Condición: `vr = vl`
- Resultado: el robot avanza en línea recta.

### 2. Movimiento curvo
- Condición: `vr ≠ vl`
- Resultado: el robot describe una trayectoria curva.

### 3. Rotación en el lugar
- Condición: `vr = -vl`
- Resultado: el robot gira sobre su propio eje.

---

## Resultados

- Se comprobó que pequeñas diferencias en las velocidades generan curvas suaves.
- Cuando las velocidades son opuestas, el robot rota sin desplazarse.
- El control preciso de velocidades permite generar trayectorias específicas.



---

## Análisis

- **¿Qué ocurre cuando ambas ruedas tienen la misma velocidad?**  
  El robot se mueve en línea recta.

- **¿Cómo cambia la trayectoria cuando las velocidades son diferentes?**  
  El robot describe una curva, cuyo radio depende de la diferencia de velocidades.

- **¿Qué ocurre cuando una rueda gira en sentido opuesto a la otra?**  
  El robot rota en su propio eje.

- **¿Qué tipo de movimiento permite dibujar un círculo?**  
  Velocidades constantes pero diferentes (`vr ≠ vl`).

---

## Desafíos implementados

- Movimiento en línea recta ✅
- Movimiento en curva ✅
- Movimiento circular ✅
- (Opcional) Otras figuras ⬜

---

## Integrantes

- Programador:  
- Experimentador:  
- Analista:  
- Documentador:
- Integrador:  

---

## Contenido del repositorio

- Código del controlador del robot
- Archivos de simulación
- README.md
- Evidencia (imágenes o videos)

---
