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
**Localization scan:** [Scan dialogue for banned honorifics: -chan, -san, -kun, -sama, -senpai, -sensei, -kouhai / Whitelist: Choco-sen, Choco-sensei, Iroha-dono, Gozaru-dono, Mio-mama, verbal tics / Log fixes if any]
```
Extra Regex:
```
/(?<!Choco)-sen(?:sei)?(?=\b)|(?<!Mio)-mama\b|(\w+)-(chan|san|kun|sama|senpai|kouhai)\b/g
```

