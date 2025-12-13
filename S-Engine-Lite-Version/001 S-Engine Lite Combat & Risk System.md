### **S-Engine Lite: Combat & Risk System**

**[License & Attribution]**

- **Copyright:** This file belongs to **ShadowK**.
- **Usage:**
  - Personal use is free.
  - Commercial use is permitted.
  - **Requirement:** If you develop a game using the numerical values from this engine, you must explicitly state in the game logic that you referenced **ShadowK's materials**.

------

### **Internal Energy Unit & Multiplier Definition (Core Rule)**

> **Internal Energy Unit Definition**
>
> In this system, **1 Internal Energy Unit is strictly defined as the Cost value specified in the Skill Tree & Leveling System**.
>
> Accordingly:
>
> - **Cost 1 = 1 Internal Energy Unit**
> - **Cost 2 = 2 Internal Energy Units**, and so on.
>
> Based on the Growth & Class System multipliers:
>
> - **1 Internal Energy Unit corresponds to 30 points of Internal Energy**,
> - **Total Internal Energy is calculated as (Cultivation Years × 100)**,
> - **Total Health is calculated as (Cultivation Years × 30)**.
>
> All combat-related energy consumption, recovery, and depletion are resolved using this unified Unit-based conversion rule.

-----

### **1. In-Game Time Settings**

- **Daily Cycle:** The day is divided into 05:00, 13:00, and 21:00 (Real-time).
- **Time Ratio:** One day in reality equals three days in the game (1:8 ratio).

------

### **2. Cultivation (Qi Accumulation) & Internal Injury**

#### **Attack Speed Settings**

- **Realm Progression:** Ranks ascend in the order of: Third Rate (a) → Second Rate (b) → First Rate (c) → Peak (d) → Super Peak (e) → Transcendent (f) → Profound (g) → Life & Death (h) → Nature (i).
- **Speed Formula:** Square root values ($\sqrt{1}, \sqrt{2}, \sqrt{3}, \dots, \sqrt{9}$) are assigned as attack speed multipliers for each rank.
- **Definition:** Attack speed is defined as the time required to perform one attack and one defense.
- **Calculation:** An attack speed of $\sqrt{1}$ is calculated as **1 attack per 3 seconds**. Subsequent values are calculated proportionally.

#### **Circulation Path (= Circulation Speed)**

- **Damage Reduction:** A ratio of `Stability / 500` is applied to reduce the damage received from Internal Injury.

------

### **3. 1 vs 1 Combat Logic**

- **First Strike:** The character with the faster **Movement Speed** initiates the first attack.
- **Subsequent Priority:** For subsequent exchanges, the character with faster **Cultivation Speed** gains attack priority after completing **100 Circulation** within one exchange.
  - *Note:* Attack priority may change if the character is controlled by a player.
- **Clash Calculation:** When attacks clash, the **Circulation Progress** is calculated based on attack speed.
  - *(Example: If the Superior Rank takes 2s and the Opponent takes 3s, when the Superior attacks, the Opponent has completed **66.7%** of their Circulation Path.)*

#### **Penalties**

1. **Rank Gap:** For every 1 rank difference, a **-3%** penalty is applied to the lower rank's **Attack Power** and **Defense**.
2. **Heart Method (Mental Arts) Gap:** If there is a difference in Heart Method grades:
   - Additional **-3%** penalty to Attack/Defense per grade.
   - Additional **-3%** penalty to **Attack Speed** per grade.

#### **Combat Flow (Crucial)**

- **(Important)** An attacker can only initiate an attack when the **Circulation Path is at 80 or above**.
- The defender executes an **automatic defense** against the attack.
- **Internal Injury:** Both the attacker and defender receive damage based on **Internal Injury Energy** if they fail to reach 100 on the Circulation Path before the action.

#### **Damage Distribution**

- **Default Setting:** Damage is split as **30% to Health (HP)** and **70% to Internal Energy (MP)**.
- *Note:* This ratio is adjustable by the user.

#### **Incapacity & Escape (Triage Logic)**

- Opportunities for **'Combat Incapacity'** or **'Escape'** decisions are triggered based on the ratio of **Used Internal Energy** to **Total Internal Energy**.
- **Thresholds based on Remaining Internal Energy:**
  - **Basic / Standard / Advanced Heart Methods:** Trigger at **40%** remaining.
  - **Secret Arts (Esoteric Methods):** Trigger at **30%** remaining.

------

### **4. Core Formulas (The Logic Engine)**

- `Circulation Path` = $\sqrt{\text{Cultivation Speed}}$
- `Circulation Risk` = $1 \div (\sqrt{\text{Stability}})$
- `Remaining Circulation` = $100 - \text{Circulation Progress}$
- `Skill Destructive Power` = $\text{Circulation Path} \times (\text{Circulation Progress} / 100)$
- `Attack Energy` = $\text{Consumed Energy} + \text{Internal Injury Energy}$
- `Consumed Energy` = $\text{Circulation Progress} \times \text{Circulation Risk}$
- `Internal Injury Energy` = $\text{Remaining Circulation} \times \text{Circulation Risk}$
- `Accumulation Injury Energy` = $\text{Internal Injury Energy}$

Final Damage Application:

Damage derived from Skill Destructive Power + added values is applied as 30% to HP and 70% to Internal Energy. (User adjustable).