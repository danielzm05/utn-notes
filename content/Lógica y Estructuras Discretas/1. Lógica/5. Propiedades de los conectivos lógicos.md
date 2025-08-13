
> [!important] Title
> Si dos proposiciones son equivalentes se escribe p ⇔ q o bien p ≡ q

#### Involución
- *~(~p) ⇔ p*

#### Idempotencia
- (p ∨ p) ⇔ p
- (p ∧ p) ⇔ p
#### Conmutatividad
- *(p ∨ q) ⇔ (q ∨ p)*
- *(p ∧ q) ⇔ (q ∧ p)*
- *(p ⇔ q) ⇔ (q ⇔ p)*
#### Absorción
- *p ∧ (p ∨ q) ⇔ p*
- *p ∨ (p ∧ q) ⇔ p*
#### Identidad
- *p ∧ V ⇔ p*
- *p ∨ F ⇔ p*

#### Dominación
- *p ∧ F ⇔ F*
- *p ∨ V ⇔ V*

#### Leyes de De Morgan
- *¬(p ∧ q) ⇔ (¬p ∨ ¬q)*
- *¬(p ∨ q) ⇔ (¬p ∧ ¬q)*

#### Asociatividad
- *(p ∨ (q ∨ r)) ⇔ ((p ∨ q) ∨ r)*
- *(p ∧ (q ∧ r)) ⇔ ((p ∧ q) ∧ r)*

#### Distributiva
- *p ∧ (q ∨ r) ⇔ (p ∧ q) ∨ (p ∧ r)*
- *p ∨ (q ∧ r) ⇔ (p ∨ q) ∧ (p ∨ r)*

---
#### Otras definiciones

##### Condicional
**En** `p ⇒ q`:
- `p` es el **antecedente**
- `q` es el **consecuente**

A partir de `p ⇒ q`, se pueden construir:

- **Recíproca:** `q ⇒ p`
- **Contra recíproca:** `~q ⇒ ~p`
- **Contraria:** `~p ⇒ ~q`

- `~p ⇒ ~q` ≡ `q ⇒ p`
- `p ⇒ q` ≡ `~p ∨ q`
##### Bicondicional

A partir de `p ⇔ q`, se pueden construir:

- `p ⇔ q` ≡ `(p ⇒ q) ∧ (q ⇒ p)`  
  También se puede expresar como:  
  `p ⇔ q` ≡ `(~p ∨ q) ∧ (~q ∨ p)`