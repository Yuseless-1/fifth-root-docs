!!! note "Early technical draft (Feb 2026)"
    Kept for reference. Where it disagrees with the main chapters, the main chapters are current.

---

# **Dice System — Full Specification**

The Dice System is the core randomization engine of Fifth Root’s combat. It determines accuracy, damage variance, critical hits, defensive blocks, ability triggers, and special events. Dice ensure that battles remain dynamic while still rewarding strategy, stats, and build choices.

--------------------

## **1. Dice Types & Their Roles**

| Dice | Use Case | Description |
|------|----------|-------------|
| **D6** | Basic attacks | Determines hit/miss, damage variance |
| **D8** | Ability triggers | Used for activation checks and conditional effects |
| **D12** | Critical rolls | Determines crit chance and crit severity |
| **D20** | Rare events | Escape attempts, ultimate triggers, environmental effects |

Each die type is tied to a specific category of combat action to keep outcomes predictable and readable.

--------------------

## **2. Core Dice Mechanics**

### **2.1 Attack Rolls (D6)**
Every attack uses a D6 roll:

- **1–2** → Miss  
- **3–4** → Normal hit  
- **5–6** → Strong hit (+10–20% bonus damage)

Modifiers may shift these thresholds.

### **2.2 Ability Activation (D8)**
Abilities that require a trigger roll use a D8:

- **1–3** → Ability fails  
- **4–7** → Ability activates normally  
- **8** → Enhanced activation (bonus effect)

### **2.3 Critical System (D12)**
Critical hits are determined by rolling a D12:

- **1–9** → No crit  
- **10–11** → Minor crit (1.5× damage)  
- **12** → Major crit (2× damage + effect)

Guild bonuses, accessories, and abilities can modify crit thresholds.

### **2.4 Rare Events (D20)**
Used for:

- Escape attempts  
- Ultimate ability triggers  
- Environmental effects  
- Raid‑scale mechanics  

**Natural 20** always succeeds.  
**Natural 1** always fails.

--------------------

## **3. Dice Modifiers**

Modifiers come from:

- Player stats  
- Sprite stats  
- Accessories  
- Abilities  
- Guild bonuses  
- Status effects  

Modifiers can:

- Increase die size (D6 → D8)  
- Add flat bonuses (+1 to roll)  
- Shift thresholds (e.g., crit on 9+)  
- Add rerolls  

--------------------

## **4. Reroll System**

Rerolls are powerful and limited.

Sources include:

- Energy guild bonuses  
- Certain accessories  
- High‑rank abilities  

Rules:

- You may only reroll **once per category** (attack, defense, crit)  
- You must keep the second result  

--------------------

## **5. Multi‑Dice Mechanics**

Some abilities roll multiple dice:

- **Take highest** (offensive abilities)  
- **Take lowest** (defensive abilities)  
- **Sum dice** (rare, high‑impact abilities)  

--------------------

## **6. Dice Transparency**

All rolls are visible to both players to maintain fairness and clarity.

---