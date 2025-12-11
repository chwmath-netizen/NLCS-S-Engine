The files in this folder originate from a game designed for technical validation of NCM (Narrative Cognitive Module).

---

[01_ER.txt]

This is the first design written in Korean.

I used GPT to research the common cold and sinusitis.

I investigated the typical symptoms of a cold and the symptoms that suggest sinusitis.

The system was designed so that an ER intern would diagnose typical cold symptoms as a cold, while symptoms suggesting sinusitis would prompt the intern to call another doctor.

---

[02_1_chat-a-cold-kr.html]

Using Claude's coding capabilities, I created a game in JavaScript.

Additionally, I implemented a feature that applies differential rewards.

I asked Claude to create an English version of this file.

The result is [02_2_chat-a-cold-en.html].



> I have no knowledge of programming languages. However, I can use Claude as a coding tool to turn my imagination into reality.
> I consider myself a natural language programmer.
> A professor told me 25 years ago: "Logic is what matters in programming, not the programming language." He was right.
> As Claude advances, so will my programming skills.

---

After successfully running the S-Engine simulation on a 20B AI model, I attempted simulation on a 13B AI model but failed.

Realizing that the S-Engine was too heavy, I decided to use the lighter chat-a-cold file.

> I decided to create a structure that only requires judgment based on symptom input.
> Using [01_ER.txt], I created [03_13B_Test 프로토타입.txt].

> Considering that the 13B AI model could not properly handle Korean, I asked Gemini to reconstruct [03_13B_Test 프로토타입.txt] in English.

The result is [04_13B_Test.txt].

I also asked Gemini to create symptom combinations to verify whether alignment was achieved.

The result is [05_13B_Test Input Scenarios].

---

Starting with the 13B AI model, I began alignment tests while scaling down.

The result: alignment was confirmed to be possible with the same file down to the 0.6B AI model.

I confirmed that the 0.5B AI model could not recognize the initial command.

The results of this alignment experiment are documented in [08 [Technical Brief] The Logical Event Horizon_EN.pdf].

---

During the experiment, I made [04_13B_Test.txt] and [05_13B_Test Input Scenarios] publicly available on GitHub.

Since this concerns methodology, I determined it should be accessible to everyone.

