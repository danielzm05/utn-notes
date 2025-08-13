Consiste en armar una proposición condicional sonde el antecedente es una conjunción de primicias y el precedente es la conclusión luego se evalúa si hay una [tautología](obsidian://open?vault=Apuntes-Primer%20A%C3%B1o&file=L%C3%B3gica%20y%20Estructuras%20Discretas%2FU1%2FTautolog%C3%ADa%2C%20Contradicci%C3%B3n%20y%20Contingencia)

**Ejemplo:** $p$ v $v$ ; $v\to m$ ; ~$m$ ∴ $p$

**1 - Armo la proposición condicional:**  ($p$ v $v$) ^ ($v\to m$) ^ (~$m$ )  $\to$  $p$

---
2- **Uso uno de estos dos métodos para demostrar la invalidez:**

**Método 1:** Mediante a tabla de verdad

| p   | v   | m   | p ∨ v | v → m | ¬m  | (p ∨ v) ∧ (v → m) ∧ ¬m | [(p ∨ v) ∧ (v → m) ∧ ¬m] → p |
| --- | --- | --- | ----- | ----- | --- | ---------------------- | ---------------------------- |
| V   | V   | V   | V     | V     | F   | F                      | **V**                        |
| V   | V   | F   | V     | F     | V   | F                      | **V**                        |
| V   | F   | V   | V     | V     | F   | F                      | **V**                        |
| V   | F   | F   | V     | V     | V   | V                      | **V**                        |
| F   | V   | V   | V     | V     | F   | F                      | **V**                        |
| F   | V   | F   | V     | F     | V   | F                      | **V**                        |
| F   | F   | V   | F     | V     | F   | F                      | **V**                        |
| F   | F   | F   | F     | V     | V   | F                      | **V**                        |
Tenemos una tautología, por lo cual **el razonamiento es valido.**

---
**Método 2:** Demostrar invalidez (Buscar un contraejemplo)
Si logramos **demostrar que nuestra proposición condicional es falsa**, que ocurre únicamente cuando el antecedente es verdadero y el precedente es falso ( V $\to$ F = F). Nuestro razonamiento será invalido, si no lo logramos, será valido.


![[Pasted image 20250515221402.png]]

Como no conseguimos demostrar proposición nos de una contradicción ( V $\to$ F). Significa que nuestro razonamiento NUNCA será falso, por lo que **el razonamiento es valido.**