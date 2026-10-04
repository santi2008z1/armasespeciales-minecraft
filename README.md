# Armas Especiales (Special Weapons)

Mod para **Minecraft Java 1.20.1** con **Fabric**.

## Armas
| Arma | Daño | Vel. ataque | Efecto |
|---|---|---|---|
| Espada de Fuego | 8 | 1.6 | Prende fuego 4 s + partículas de llama |
| Martillo de Guerra | 9 | 0.9 | Empuja hacia atrás + partículas y sonido |
| Daga | 4 | 2.7 | Ataque muy rápido |
| Arco Mágico | como arco | como arco | Flechas +1 daño, Lentitud 2 s y Brillo 5 s |
| Espada de Relámpago | 7 | 1.6 | 15 % de invocar un rayo (5 de daño, sin dañar al jugador) |

## Recetas
- Espada de Fuego: ` D ` / `CDC` / ` I ` (D=diamante, C=carbón, I=hierro)
- Martillo de Guerra: `III` / `IDI` / ` I `
- Daga: 2 lingotes de hierro en vertical
- Arco Mágico: ` D ` / `LBL` / ` D ` (L=lapislázuli, B=arco)
- Espada de Relámpago: ` D ` / `RDR` / ` I ` (R=redstone)

## Compilar
Requisitos: **JDK 17** y **Gradle 8.5+** (con conexión a internet).

```
gradle wrapper --gradle-version 8.5   # solo la primera vez (genera gradlew)
./gradlew build                        # en Windows: gradlew.bat build
```
El mod queda en `build/libs/specialweapons-1.0.0.jar` (no uses el `-sources.jar`).

Alternativa sin instalar nada: sube la carpeta a un repositorio de GitHub; el workflow
`.github/workflows/build.yml` compila y deja el `.jar` como artefacto descargable.

## Instalar
1. Instala Fabric Loader para 1.20.1 y **Fabric API**.
2. Copia el `.jar` a la carpeta `mods`.

## Ajustar el equilibrio
Números en `ModToolMaterials.java` y en el constructor de cada clase de `item/`.
