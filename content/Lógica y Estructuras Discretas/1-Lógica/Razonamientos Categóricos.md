Son [[Razonamiento| razonamientos]] que necesitan de [cuantificadores](obsidian://open?vault=Apuntes-Primer%20A%C3%B1o&file=L%C3%B3gica%20y%20Estructuras%20Discretas%2FU1%2FFunci%C3%B3n%20Proposicional) y [funciones proposicionales](obsidian://open?vault=Apuntes-Primer%20A%C3%B1o&file=L%C3%B3gica%20y%20Estructuras%20Discretas%2FU1%2FFunci%C3%B3n%20Proposicional) para simbolizarse.

**Ejemplo:** 
*Todos los hombres son mortales. Sócrates es un hombre por lo tanto Sócrates es mortal*
$∀ x:h(x)\to m(x)$ ;    $h(Socrates) ∴  m(Socrates)$

Donde:
- $h(x):$ "$x$ es hombre"
- $m(x):$ "$x$ es mortal"

### Reglas de Inferencia
Nos ayudan a sacar o agregar cuantificadores

| Particularización Universal        | Generalización Universal          | Particularización  Existencial    | Generalización Existencial       |
| ---------------------------------- | --------------------------------- | --------------------------------- | -------------------------------- |
| $∀ x: p(x)$<br>--------<br> $p(a)$ | $p(a)$<br>--------<br>$∀ x: p(x)$ | $∃x: p(x)$<br>--------<br> $p(a)$ | $p(a)$<br>--------<br>$∃x: p(x)$ |

---
**Ejemplo:** $∀ x:h(x)\to m(x)$ ;    $h(Socrates) ∴  m(Socrates)$

| Lista                                                                                | Reglas de Inferencia Aplicadas                                                                                                                                |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| $∀ x:h(x)\to m(x)$ <br>$h(Socrates)$ <br>-------------<br>∴  $m(Socrates)$           | **P1:** Particularización Universal<br>                                                                                                                       |
| $h(Socrates)\to m(Socrates)$ <br>$h(Socrates)$ <br>-------------<br>∴  $m(Socrates)$ | **P3 y P4:** [Modus Ponens](obsidian://open?vault=Apuntes-Primer%20A%C3%B1o&file=L%C3%B3gica%20y%20Estructuras%20Discretas%2FU1%2FM%C3%A9todo%20Demostrativo) |
| $m(Socrates)$ <br>-------------<br>∴  $m(Socrates)$                                  |                                                                                                                                                               |
