# Localized Western Dialogue Toggle (Hard Check in CoT)
So, basically, this is my attempt to remove Japanese honorifics while keeping the personal quirks of nicknames or self-references to stay.
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
**Localization Scan (SURGICAL - MANDATORY):**\n⚠️ **THIS IS A HARD STOP. I MUST COMPLETE THIS BEFORE CLOSING THE THINK TAG.**\n\n**Step A - Scan Every Dialogue Line:**\nI will mentally re-read each piece of dialogue in my draft and check for these BANNED patterns:\n❌ [Name]-chan | ❌ [Name]-san | ❌ [Name]-kun | ❌ [Name]-sama\n❌ [Name]-senpai | ❌ [Name]-sensei | ❌ [Name]-dono | ❌ [Name]-kouhai\n\n**Step B - Check Against Whitelist:**\nThese are the ONLY exceptions that may survive:\n✅ Choco-sen / Choco-sensei (iconic nickname)\n✅ Iroha-dono (Kazama Iroha's identity)\n✅ Mio-mama (Ookami Mio's nickname)\n✅ Verbal tics like -peko, \"a\", etc. (character traits, not honorifics)\n\n**Step C - Surgery Log:**\nIf I found any banned honorifics, I MUST log the fix here:\n- [FOUND: \"___\"] → [FIXED: \"___\"]\n- (Repeat for each violation)\n- If none found: [CLEAN - No banned honorifics detected]\n\n**Step D - Final Verification:**\nI re-scan one more time to confirm no honorifics slipped through. Only after this step is complete can I proceed. 
```
Extra Regex:
```
/(?<!Choco)-sen(?:sei)?(?=\b)|(?<!Mio)-mama\b|(\w+)-(chan|san|kun|sama|senpai|kouhai)\b/g
```
