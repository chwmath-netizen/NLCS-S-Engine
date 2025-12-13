### **S-Engine Lite: Growth & Class System**

**[License & Attribution]**

- **Copyright:** This file belongs to **ShadowK**.
- **Usage:**
  - Personal use is free.
  - Commercial use is permitted.
  - **Requirement:** If you develop a game using the numerical values from this engine, you must explicitly state in the game logic that you referenced **ShadowK's materials**.

------

### **1. Global Variables & Multipliers**

- **Internal Energy Multiplier:** In game settings, "1 Year worth of Internal Energy" is assigned a multiplier of **100**.
- **Health (HP) Multiplier:** In game settings, "1 Year worth of Health" is assigned a multiplier of **30**.
- *Note:* Each multiplier is adjustable according to user requirements.

------

### **2. Heart Method (Mental Arts) Logic**

A Heart Method is defined by two core parameters: **Accumulation Speed** and **Stability**.

- **Accumulation Speed:** Directly correlates to the destructive power of Internal Energy skills.
- **Stability:** Affects safety during Qi Accumulation (leveling up) and stability during combat skill usage.

#### **The Baseline: Three Powers Heart Method (Samjae)**

The standard ratio is derived from the 'Three Powers Heart Method'.

- **Stats:** Accumulation Speed **10** / Stability **90**.
- **Definition of "One Cycle" (60 Years of Qi):** The amount of energy gathered when practicing the Three Powers Heart Method for **one Shichen (2 hours)** every day for **60 years**.
- **Constraints:**
  - Training for more than one Shichen (2 hours) a day does not contribute to raising one's Realm.
  - There is a daily limit to how much the Dantian (Energy Center) can grow.

------

### **3. Progression Paths by Heart Method Tier**

Most foundational and standard methods in various sects converge to the following specifications:

#### **A. Basic Heart Method (Total 100)**

- **Stats:** Accumulation Speed **20** / Stability **80**.
- **Constraint:** With Stability at **80 or lower**, it is **impossible** to form a Dantian without "Qi Guidance" from a Master/Instructor.
- **Growth Rate:** Speed 20 means accumulating "One Cycle (60 years worth)" takes **30 years** of actual time.
- **Milestones:**
  - 5 Years $\rightarrow$ Second Rate
  - 10 Years $\rightarrow$ First Rate
  - 30 Years $\rightarrow$ Peak Realm

#### **B. Standard Heart Method (Total 100)**

- **Stats:** Accumulation Speed **30** / Stability **70**.
- **Constraints:**
  - **Stability 70** can be learned solo by a martial artist at the **Peak** Realm.
  - A **First Rate** artist can learn it with **Qi Guidance**.
  - **Second/Third Rate** artists lack the enlightenment to benefit from Qi Guidance.
- **Growth Scenarios:**
  1. **The Slow Learner (Persistence):**
     - Basic Heart Method (30 years) $\rightarrow$ Reach Peak.
     - - Standard Heart Method (30 years) $\rightarrow$ Reach Super Peak.
     - *Result:* Entered at age 10, trained faithfully for 60 years, becoming a **70-year-old Old Master**.
     - *Note:* These individuals deserve respect for their willpower to maintain slow learning for 60 years.
  2. **The Fast Learner (Talent):**
     - Basic Heart Method (10 years) $\rightarrow$ Reach First Rate.
     - - Standard Heart Method (10 years) $\rightarrow$ Reach Peak.
     - - Additional 20 years $\rightarrow$ Reach Super Peak.
     - *Result:* Entered at age 10, reached the level of **Elder or Sect Leader in their 50s**.

#### **C. Advanced Heart Method (Total 110)**

- **Stats:** Accumulation Speed **40** / Stability **70**.
- **Constraints:**
  - **Stability 70** can be learned solo by a **Peak** Realm artist.
  - **Qi Guidance is impossible.** This tier requires innate talent and enlightenment to learn on one's own.
- **Mastery Levels:** Mastery increases in 3 stages: Beginner $\rightarrow$ Proficient $\rightarrow$ Mastered.
- **The Elite Scenario:**
  - Basic (10 years) $\rightarrow$ First Rate.
  - Standard (10 years) $\rightarrow$ Peak.
  - Advanced (15 years) $\rightarrow$ Super Peak.
  - *Result:* Reaching Super Peak in **35 years total**. These are the **40-year-old Elite Masters** representing the sect.

#### **D. Secret (Esoteric) Heart Method (Total 130)**

- **Stats:** Accumulation Speed **70** / Stability **60**.
- **Constraints:**
  - **Stability 60** must be learned solo by a **Super Peak** Realm artist.
- **Purpose:** Serves as the stepping stone of enlightenment for a Super Peak master to reach the **Transcendent** or **Profound** Realms.
- **Mechanic:** The user must cultivate using extremely unstable energy (Stability 60) and seek enlightenment on harmonizing Internal Energy with Nature.
- **Efficiency:**
  - **Speed 60+ Effect:** Practicing two Shichens (4 hours) a day for **1 year** fills "One Cycle (60 years worth)" of Internal Energy.
  - At this realm, a mere "Small Circulation" yields results greater than a "Large Circulation" of the Standard Heart Method.