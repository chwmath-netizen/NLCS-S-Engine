### **S-Engine Lite: Footwork & Movement System**

**[License & Attribution]**

- **Copyright:** This file belongs to **ShadowK**.
- **Usage:**
  - Personal use is free.
  - Commercial use is permitted.
  - **Requirement:** If you develop a game using the numerical values from this engine, you must explicitly state in the game logic that you referenced **ShadowK's materials**.

------

### **1. Footwork Mastery Tiers**

- **Basic Footwork:** Stage 1, 2, 3 $\rightarrow$ **Lv1, Lv2, Lv3**
- **Standard Footwork:** Stage 1, 2, 3 $\rightarrow$ **Lv4, Lv5, Lv6**
- **Advanced Footwork:** Stage 1, 2, 3 $\rightarrow$ **Lv7, Lv8**

------

### **2. Acquisition Limits by Realm**

A character's martial realm limits the maximum level of Footwork they can master.

- **Third Rate:** Capable of Lv1, Lv2.
- **Second Rate:** Capable of Lv1 ~ Lv3.
- **First Rate:** Capable of Lv1 ~ Lv4.
- **Peak Realm:** Capable of Lv1 ~ Lv5.
- **Super Peak Realm:** Capable of Lv1 ~ Lv6.
- **Transcendent (Hwagyeong):** Capable of Lv1 ~ Lv7.
- **Profound (Hyeongyeong):** Capable of Lv1 ~ Lv8.

------

### **3. Learning Path**

Footwork is acquired through **Footwork Manuals**.

- **Basic Manuals:** Teaches Lv1 / Lv2 / Lv3.
- **Standard Manuals:** Teaches Lv4 / Lv5 / Lv6.
- **Advanced Manuals:** Teaches Lv7 / Lv8.

------

### **4. Mechanics: Speed & Combat Application**

#### **Movement Speed Calculation**

- Multipliers are applied to the character's **Base Running Speed** based on Footwork Level.
- **Formula:** $\sqrt{1}, \sqrt{2}, \sqrt{3}, \sqrt{4}, \sqrt{5}, \sqrt{6}, \sqrt{7}, \sqrt{8}$.
  - *(Example: Lv4 Footwork increases speed by a factor of $\sqrt{4} = 2$.)*

#### **Combat Bonus (Linkage)**

- When **Footwork is linked with Attacks** during combat, additional damage is applied to the **Destructive Power of Internal Energy Arts**.
- **Bonus Damage:** 10%, 20%, ... up to 90% based on proficiency level.

------

### **5. Basic Movement Controls**

Supports **8-Directional Movement**:

- Forward
- Forward-Left, Forward-Right
- Left, Right
- Backward
- Backward-Left, Backward-Right