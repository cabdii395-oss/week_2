# Week 2 Tutorial: Movie Theater Admission Policy

---

## 1. Identify the Components

* **1.1. Inputs:**
    * `age` (Integer: The age of the moviegoer)
    * `has_adult` (Boolean: True if accompanied by an adult, False if alone)
    * `has_ticket` (Boolean: True if they have a valid ticket, False if they do not)
* **1.2. Process:** * Check if the user possesses a valid ticket (`has_ticket == True`).
    * If they have a ticket, verify if they meet either age requirement (`age >= 13`) OR supervision requirement (`has_adult == True`).
* **1.3. Output:** * Admission status message (e.g., "Allowed to enter" or "Not allowed to enter").

---

## 2. Design the Algorithm

### 2.1 Diagram
*(Once you export your flowchart image from draw.io/Canva, save it in this directory and reference it here)*
![Flowchart Diagram](image.png)

### 2.2 Truth Table

| Ticket? (`has_ticket`) | Age $\ge$ 13? | With Adult? (`has_adult`) | Logical Expression: `has_ticket AND (age >= 13 OR has_adult)` | Output (Allowed?) |
| :---: | :---: | :---: | :---: | :---: |
| **False** | False | False | $\text{False} \land (\text{False} \lor \text{False}) = \text{False}$ | **No** |
| **False** | True | True | $\text{False} \land (\text{True} \lor \text{True}) = \text{False}$ | **No** |
| **True** | False | False | $\text{True} \land (\text{False} \lor \text{False}) = \text{False}$ | **No** |
| **True** | **True** | False | $\text{True} \land (\text{True} \lor \text{False}) = \text{True}$ | **Yes** |
| **True** | False | **True** | $\text{True} \land (\text{False} \lor \text{True}) = \text{True}$ | **Yes** |
| **True** | **True** | **True** | $\text{True} \land (\text{True} \lor \text{True}) = \text{True}$ | **Yes** |

> *Note: If `has_ticket` is False, the entire expression breaks down to False instantly because a ticket is strictly required.*

### 2.3 The Step-by-Step Solution (Algorithm)
1. Start the program.
2. Prompt and capture the user's input for `age`, `has_adult`, and `has_ticket`.
3. Evaluate if `has_ticket` is equal to True.
4. If True, check if `age` is greater than or equal to 13, OR if `has_adult` is equal to True.
5. If either condition in step 4 is true, display "Allowed to enter".
6. If conditions in step 4 are false, or if step 3 is false, display "Not allowed to enter".
7. End the program.

### 2.4 Pseudocode
```text
START
    INPUT age
    INPUT has_adult
    INPUT has_ticket

    IF has_ticket == True THEN
        IF age >= 13 OR has_adult == True THEN
            OUTPUT "Allowed to enter"
        ELSE
            OUTPUT "Not allowed to enter"
        ENDIF
    ELSE
        OUTPUT "Not allowed to enter"
    ENDIF
END