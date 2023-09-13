## IA
### Tic Tac Toe 3D
- Estrategia de percepción:
    - Analizar y observar las 3 distintas capas del tablero para percibir si el oponente se está enfocando en alguna capa en específico.
    - Bloquear jugadas clave, cuando existan dos simbolos del oponente de la forma (x, y+1), (x, y-1), (x+1, y), (x-1, y), (x+1, y+1),(x-1, y+1), (x+1, y-1) o (x-1, y-1).
    - De no existir jugadas que bloquear, se buscará generar oportunidades de ganar colocando el simbolo de una forma como los ejemplos anteriores para asi poder estar generando oportunidades y mantener al oponente a la defensiva.
    - Si se cuenta con dos simbolos ya colocados como los ejemplos anteriores, entonces lo que se hará es verificar si hay un espacio en ese mismo nivel de estar los dos simbolos en un mismo nivel, o en el siguiente nivel si se encuentran entre distintos niveles.
    - Una jugada clave que se debe buscar crear es una que posea una victoria por ambos caminos a la vez. Esta jugada se puede obtener buscando la formación de una "L" con los simbolos, ya sea en un solo nivel o entre los tres a la vez y asi poder obtener la victoria.

- Medida de rendimiento:
    - Ganar:
        - Se gana en el momento en que se forma una línea de tres simbolos en cualquiera de las direcciones válidas que serían: horizontal, vertical, en profundidad o en diagonal.
    - Empate:
        - El juego termina en empate cuando todas las casillas de los tableros se encuentran ocupados y ninguno de los jugadores haya logrado formar una línea ganadora.