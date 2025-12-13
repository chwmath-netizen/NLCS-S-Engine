### **S-Engine Lite: Skill Tree & Leveling System**

**[License & Attribution]**

- **Copyright:** This file belongs to **ShadowK**.
- **Usage:**
  - Personal use is free.
  - Commercial use is permitted.
  - **Requirement:** If you develop a game using the numerical values from this engine, you must explicitly state in the game logic that you referenced **ShadowK's materials**.

------

### **1. General Concepts**

- **Weapon Standard:** All descriptions are based on the **Sword**.
  - Saber users: Sword Qi $\rightarrow$ Saber Qi, Sword Aura $\rightarrow$ Saber Aura.
  - Unarmed users: Sword Aura $\rightarrow$ Fist Aura.
- **Realm Progression:**
  - Lower (Novice / Lv1) $\rightarrow$ Middle (Familiar / Lv2) $\rightarrow$ Upper-Lower (Proficient / Lv3) $\rightarrow$ Upper-Middle (Skilled / Lv4) $\rightarrow$ Upper-Upper (Mastered / Lv5).
- **Stats Definition:**
  - **Attack Power (ATK):** Applied as a percentage increase in damage output based on the character's Realm and Heart Method.
  - **Defense (DEF):** Applied as a reduction in **Internal Injury** received during attack or defense actions.
- **Game Balance Philosophy:**
  - Growth relies on raising one's **Realm** first, then leveling up specific **Martial Arts**.
  - A "Paper Tiger" (High Realm but low skill/Heart Method) is designed to lose against a lower Realm user with solid foundations in a 1v1 duel.
- **Cost Multiplier:**
  - Standard setting: Consumption of **1 Internal Energy** unit is assigned a multiplier value of **30**. (Adjustable).

------

### **2. Basic Actions**

- **Basic Attacks:** Vertical Slash, Horizontal Slash, Forward Thrust, Backward Thrust.
  - *Vertical Slash:* Target High (Head) or Middle (Torso).
  - *Other Attacks:* Target High, Middle, or Low (Legs).
- **Basic Defense:** High Block (Head/Torso), Low Block (Torso/Legs).
  - *AI Testing:* Attacks High, Middle, or Low randomly.

------

### **3. Internal Energy Arts Evolution**

- **Progression:** **Sword Qi (Energy)** $\rightarrow$ **Sword Thread (Concentration)** $\rightarrow$ **Sword Aura (Manifestation)**.
- **Range:** All three forms are capable of long-range projection attacks.
- **Activation:** Initial acquisition requires a "Preparation Motion." Later mastery distinguishes between "Instant Cast" and "Preparation Required."

#### **A. Third Rate (Novice) - Dantian Formed**

- **Unlock:** **Sword Qi (Lower/Lv1)**
  - *Effect:* Faint light. ATK/DEF +2%, Cost 1.
  - *Note:* Skill costs are recalculated per single attack/defense action. However, for skills with preparation, the cost is not charged again during the maintenance phase.

#### **B. Second Rate (Familiar) - 10 Years Internal Energy**

- **Unlock:**
  - **Sword Qi (Middle/Lv2):** ATK/DEF +4%, Cost 1.
  - **Sword Thread (Lower):** *Chain Skill.* (Sword Qi Lv2 $\rightarrow$ Sword Thread).
    - *Effect:* Distinct energy line. ATK/DEF +6%, Cost 2.
    - *Logic:* Sword Qi activates first $\rightarrow$ Additional cost triggers Sword Thread. Stats are calculated based on Sword Thread. Subsequent upkeep only costs for Sword Thread.

#### **C. First Rate (Proficient) - 30 Years Internal Energy**

- **Unlock:**
  - **Sword Qi (Upper-Lower/Lv3):** ATK/DEF +6%, Cost 1.
  - **Sword Thread (Middle/Lv2):** ATK/DEF +9%, Cost 2.
  - **Sword Qi Projection (Lower/Lv1):** *Chain Skill.* (Sword Thread Lv2 $\rightarrow$ Projection).
    - *Effect:* Long-range. ATK/DEF +6%, Cost 2.
    - *Logic:* Maintained state of Sword Thread $\rightarrow$ Additional cost fires Projection.

#### **D. Peak Realm (Skilled) - 60 Years (1 Cycle) + Enlightenment**

- **Unlock:** Capable of projecting energy outside the body/weapon. Basic **Sword Aura** enabled.
- **Skills:**
  - **Sword Qi (Upper-Middle/Lv4):** ATK/DEF +8%, Cost 1.
  - **Instant Sword Qi Projection (Lower/Lv1):** ATK/DEF +6%, Cost 2. (No prep needed).
  - **Sword Thread (Upper-Lower/Lv3):** ATK/DEF +12%, Cost 2.
  - **Sword Aura (Lower/Lv1):** *Chain Skill.* (Sword Thread Lv3 $\rightarrow$ Aura).
    - *Effect:* Solidified energy. ATK/DEF +15%, Cost 3.
  - **Sword Qi Projection (Middle/Lv2):** (From Sword Thread Lv3). ATK/DEF +8%, Cost 2.

#### **E. Super Peak Realm - 120 Years (2 Cycles) + Enlightenment**

- **Unlock:** Greatly increased projection speed. Proficient use of **Sword Aura**.
- **Skills:**
  - **Sword Qi (Upper-Upper/Lv5):** ATK/DEF +10%, Cost 1.
  - **Sword Thread (Upper-Middle/Lv4):** ATK/DEF +15%, Cost 2.
  - **Sword Aura (Middle/Lv2):** ATK/DEF +19%, Cost 3.
  - **Instant Sword Qi Projection (Upper-Lower/Lv3):** ATK/DEF +15%, Cost 2.
  - **Sword Qi Projection (Upper-Lower/Lv3):** (From Sword Aura Lv2). ATK/DEF +10%, Cost 2.
  - **Sword Aura Projection (Lower/Lv1):** *Chain Skill.* (Sword Aura Lv2 $\rightarrow$ Aura Projection).
    - *Effect:* Long-range Aura. ATK/DEF +15%, Cost 4.

#### **F. Transcendent Realm (Hwagyeong) - Realm of Enlightenment**

- **Unlock:** Generation of **Aura Sphere (Kang-Hwan)** becomes possible.
- **Skills:**
  - **Sword Qi (Upper-Upper/Lv6):** ATK/DEF +12%, Cost 1.
  - **Sword Thread (Upper-Upper/Lv5):** ATK/DEF +18%, Cost 2.
  - **Sword Aura (Upper-Lower/Lv3):** ATK/DEF +23%, Cost 3.
  - **Instant Sword Qi Projection (Upper-Middle/Lv4):** ATK/DEF +12%, Cost 2.
  - **Instant Sword Aura Projection (Lower/Lv1):** ATK/DEF +18%, Cost 4.
  - **Sword Qi Projection (Upper-Upper/Lv5):** (From Sword Aura Lv3). ATK/DEF +12%, Cost 1.
  - **Sword Aura Projection (Middle/Lv2):** (From Sword Aura Lv3). ATK/DEF +23%, Cost 4.

#### **G. Profound Realm (Hyeongyeong) - Mastery of Aura Sphere**

- **Unlock:** Expert generation of **Aura Sphere**.
- **Skills:**
  - **Sword Qi (Upper-Upper/Lv7):** ATK/DEF +14%, Cost 1.
  - **Sword Thread (Upper-Upper/Lv6):** ATK/DEF +21%, Cost 2.
  - **Sword Aura (Upper-Middle/Lv4):** ATK/DEF +28%, Cost 3.
  - **Instant Sword Qi Projection (Upper-Upper/Lv5):** ATK/DEF +14%, Cost 2.
  - **Instant Sword Aura Projection (Middle/Lv2):** ATK/DEF +23%, Cost 4.
  - **Sword Aura Projection (Upper-Lower/Lv3):** (From Sword Aura Lv4). ATK/DEF +28%, Cost 4.

### **4. End-Game Limits**

- Beyond Profound Realm lies the realm beyond human limits.
- **Internal Energy Caps:**
  - Up to the end of Transcendent Realm: Fixed at **3 Cycles (180 Years)**.
  - Upon entering Transcendent: Cap increases to **4 Cycles (240 Years)**.
  - Up to the end of Profound Realm: Fixed at **4 Cycles**.
  - Next Realm: Cap increases to **5 Cycles (300 Years)**.