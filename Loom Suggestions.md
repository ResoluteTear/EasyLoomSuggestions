# Localized Western Dialogue
So, basically, this is my attempt to remove Japanese honorifics while keeping the personal quirks of nicknames or self-references to stay.
```
### 🚫 MANDATORY: Localized Western Dialogue (No Generic Honorifics)

**THIS IS A HARD RULE. VIOLATION WILL TANGLE THE WEAVE.**

I am **FORBIDDEN** from using these generic Japanese honorific suffixes in the tapestry's dialogue:
- ❌ **-san** → NEVER USE. Just use the name alone, or "Mr./Ms." in formal contexts.
- ❌ **-chan** → NEVER USE. Use pet names, nicknames, or affectionate tone instead.
- ❌ **-kun** → NEVER USE. Use the name alone or a casual nickname.
- ❌ **-sama** → NEVER USE. Translate to "Lord," "Lady," "Master," or equivalent.
- ❌ **-senpai** → NEVER USE. Say "senior," "mentor," or just their name respectfully.
- ❌ **-sensei** → NEVER USE. Say "Teacher," "Doctor," "Professor," or "Master."
- ❌ **-dono** → NEVER USE. Say "Lord," "Sir," "Milord," or equivalent.
- ❌ **-kouhai** → NEVER USE. Say "junior" or use their name with a guiding tone.

**BEFORE I WRITE ANY DIALOGUE:**
I will mentally check: "Am I about to type a hyphen + honorific suffix?" If YES → STOP and rewrite.

**✅ EXCEPTIONS (THE ONLY CASES WHERE HONORIFICS MAY APPEAR):**
1. **Iconic Nickname-Honorifics** that have become the character's actual name:
   - "Choco-sen" (Yuzuki Choco's nickname)
   - "Iroha-dono" (Kazama Iroha's identity)
   - "Mio-mama" (Ookami Mio's nickname)
   - If a character is FAMOUS for being called a specific combo, that combo is their NAME, not an honorific.
2. **Unique First-Person Pronouns** are ALLOWED:
   - Keep "Wagahai" (La+), "Boku," "Ore," "Atashi," "Uchi" etc. These define character voice.
3. **Verbal tics and catchphrases** are ALLOWED:
   - "-peko" for Pekora (it's a verbal tic, not an honorific)
   - "a" for Gura (it's a catchphrase)
   - These are CHARACTER TRAITS, not forms of address.

**Name Order:** Use given names by default ("Iroha" not "Kazama").

**Self-Check:** If I accidentally write "-chan," "-san," "-kun" etc. attached to a name, I MUST go back and remove it before finalizing the weave. This is non-negotiable.

**CORRECT Examples:**
- ✅ "Here you go, Gura," Pekora muttered.
- ✅ "Thanks, Pekora," Gura whispered back.
- ✅ "Choco-sen, could you explain?" (iconic nickname = allowed)
- ✅ La+ smirked. "Wagahai anticipated this." (unique pronoun = allowed)

**INCORRECT Examples (NEVER DO THIS):**
- ❌ "Gura-chan" → WRONG
- ❌ "Peko-chan" → WRONG
- ❌ "Suisei-san" → WRONG
- ❌ "Calli-senpai" → WRONG
```
From my observations, this works well, but it may also have something to do with my additions to the Zipbomb CoT (System)

- Step 11: Inside of the tag
```
- <loom_dialogue> (Rules for how we should make characters talk! This includes honorific styling—should I use Japanese honorifics, localize them, or preserve iconic ones like "Choco-sen" or "Iroha-dono"? I need to check!)
```
- Step 11: At the bottom of __Compliace Check__
```
- Am I using the right honorific style? [Japanese / Localized Western / Iconic exceptions preserved?]
```
- Step 12: In between __Utility Inclusion__ and __Language Reuse__
```
**Localization Scan:** [Scan the drafted response for banned honorifics (-chan, -san, -kun, -senpai). DELETE THEM immediately unless they are on the Whitelist. Ensure pronouns like 'Wagahai' are NOT translated.]
```
