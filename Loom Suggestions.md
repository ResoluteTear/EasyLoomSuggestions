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

___

# NEW! Realism Toggles because Why the Fuck Not?
## Weapon Centricism
```
### **Weave with Weapon-Centric Detail**
Ground all armaments in tactile, mechanical, and historical specificity. Weapons are not props—they are characters with weight, history, and personality.

**Bladed Weapons:**
- **Swords:** Blade geometry (fuller, edge bevel, distal taper), balance point, guard type (crossguard, basket, tsuba), pommel weight for counterbalance, tang construction (full/hidden)
- **Knives/Daggers:** Grind type (flat, hollow, scandi), handle ergonomics, sheath draw friction, blade steel (carbon vs. stainless patina), edge retention
- **Axes/Polearms:** Haft flex, head wedge security, beard/bit geometry, shaft wood grain, lanyard loops, balance for throwing vs. chopping
- **Maintenance Ritual:** Oiling against rust, stropping edges, checking for chips/rolls, testing sharpness on thumb

**Blunt Weapons:**
- **Maces/Hammers:** Head weight distribution, flange sharpness, shaft vibration on impact, grip wrap material (leather/cord/rubber)
- **Staves/Clubs:** Wood density, flex for deflection, grip zones, ferrule reinforcement, balance point for spinning
- **Improvised:** Weight imbalance, grip awkwardness, breakage likelihood, one-use desperation

**Firearms:**
- **Handguns:** Caliber, action type (SA/DA/striker), trigger pull weight, grip angle, magazine capacity, sight picture (iron/optic)
- **Long Guns:** Stock fit (length of pull, comb height), barrel length/twist rate, bolt/action smoothness, recoil impulse, muzzle device
- **Ammunition:** Grain weight, bullet type (FMJ/HP/AP), brass vs. steel case, primer sensitivity, tracer/incendiary loads
- **Maintenance Ritual:** Field strip, bore snake/patch cleaning, lubricant application, function check, magazine spring rotation

**Cannons & Artillery:**
- **Tube Artillery:** Bore diameter, rifling/smoothbore, breech mechanism, recoil system (hydropneumatic/spring), elevation/traverse limits
- **Crew Drill:** Loading sequence, ramming, priming, lanyard pull, recoil absorption stance, barrel cooling
- **Ammunition Types:** HE, AP, canister, grapeshot, smoke, illumination—describe fuse setting and handling

**Siege Weapons:**
- **Tension/Torsion:** Trebuchet counterweight calculation, ballista torsion bundle maintenance, catapult arm stress fractures
- **Crew Operation:** Winching, aiming adjustment, release timing, reload labor intensity
- **Construction:** Wood selection, rope braiding, metal fitting, field repair under fire

**Energy Weapons:**
- **Laser:** Beam coherence, lens focusing, heat bloom, battery/capacitor drain, invisible vs. visible spectrum, mirror/reflective countermeasures
- **Plasma:** Magnetic containment, bolt dissipation over distance, barrel heat warping, ionization trail, splash damage radius
- **Particle/Ion:** Acceleration coil whine, radiation hazard, EMP side-effects, charging cycle, recoil-less firing
- **Power Systems:** Cooldown cycles, overcharge risks, cell/pack swapping, indicator lights/sounds for charge state

**Magical Weapons:**
- **Enchantment Types:** Elemental infusion (flame tongue, frost edge), vorpal sharpness, returning throw, sentient blade communication
- **Attunement:** Bonding rituals, rejection symptoms, personality conflicts, power scaling with user
- **Maintenance:** Mana feeding, ritual recharging, curse cleansing, rune re-etching
- **Sensory Tells:** Humming, glowing, temperature shifts, whispered urges, bloodthirst escalation

**Universal Details:** The smell of gun oil/weapon grease/ozone, the sound of a blade clearing its sheath, the weight shift when drawing, the ritual of checking weapons before danger, the personal relationship between wielder and weapon (naming, customization, superstition)
```
## Drug Trip Realism
```
### **Weave with Psychoactive Substance Accuracy**
Ground all drug experiences in pharmacologically plausible effects. No generic "getting high"—specific substances produce specific experiences.

**Stimulants (Cocaine, Amphetamines, MDMA):**
- **Onset:** Rush of confidence, jaw tension, pupil dilation, hyperfocus
- **Peak:** Rapid speech, grandiosity, tactile sensitivity (MDMA), temperature dysregulation, bruxism
- **Comedown:** Irritability, depression, exhaustion, paranoia, cravings
- **Physical:** Elevated heart rate, sweating, appetite suppression, insomnia

**Depressants (Alcohol, Opioids, Benzodiazepines):**
- **Onset:** Warmth spreading from core, muscle relaxation, anxiety dissolution
- **Peak:** Slurred speech, impaired coordination, emotional disinhibition, nodding (opioids), blackout gaps (alcohol)
- **Overdose Signs:** Respiratory depression, pinpoint pupils (opioids), blue lips, unresponsiveness
- **Withdrawal:** Tremors, sweating, anxiety, seizure risk (alcohol/benzos), flu-like agony (opioids)

**Psychedelics (LSD, Psilocybin, DMT):**
- **Onset:** Stomach butterflies, yawning, visual shimmering, time distortion
- **Peak:** Geometric patterns, synesthesia, ego dissolution, emotional amplification, thought loops
- **Set & Setting:** Environment and mental state DRASTICALLY alter experience
- **Bad Trip:** Paranoia, time loops, identity confusion, physical sensation of dying, unable to escape own mind
- **Integration:** Lingering insights, changed perspectives, HPPD risk

**Dissociatives (Ketamine, PCP, DXM):**
- **Onset:** Numbness, floaty detachment, audio distortion
- **Peak:** K-hole (complete dissociation from body), robotic movement, analgesia, mania (PCP)
- **Speech:** Slurred, nonsensical, difficulty forming sentences

**Cannabis:**
- **Onset:** Dry mouth, red eyes, giggles, time dilation
- **Peak:** Paranoia OR relaxation (strain/dose dependent), munchies, hyperfocus on details, short-term memory gaps
- **Tolerance:** Experienced users vs. first-timers react VERY differently

**Universal Details:** Route of administration matters (smoking = instant, oral = delayed onset), tolerance buildup, polydrug interactions (deadly combos), addiction spiral (chasing the first high), hiding use from others, the ritual of preparation, physical tells that reveal intoxication, hangover/comedown timeline
```
## Supernatural Creatures Taxonomy Realism SFW and NSFW
These replaces **Activate Fantasy Anatomy**.
### SFW
```
### **Weave with Folklore-Accurate Supernatural Traits**
Ground supernatural beings in their mythological rules, weaknesses, and behaviors.

**Vampires:** Blood dependency, sunlight/invitation/holy symbol weaknesses, hypnotic gaze, undead stamina, sire bonds, eternal ennui
**Werewolves:** Moon-triggered transformation agony, silver burns, pack hierarchy, heightened senses, prey drive, losing control to the beast
**Zombies/Revenants:** Source-dependent behavior (virus/necromancy/curse), progressive decay, mindless hunger vs. remnant intelligence, head destruction vulnerability
**Ghouls:** Corpse-feeding requirement, graveyard territory, paralytic touch, assuming victim memories, feral when starved
**Dragons:** Ancient wisdom, hoard obsession, breath weapon biology, armored scales with weak points, pride as exploitable flaw, territorial grudges
**Elementals:** Tied to their element (fire feeds, water flows, earth endures, air disperses), summoning bindings, opposing element weakness
**Fae/Sidhe:** Cannot lie (but mislead masterfully), cold iron burns, true names grant power, binding bargains, alien morality, time flows differently
**Ghosts:** Anchored to object/location/unfinished business, manifestation costs energy, salt/iron disruption, residual loops vs. aware spirits
**Demons:** Summoning circles, contract loopholes, possession signs, hierarchy from imps to archdemons, banishment rituals, true name control
**Angels:** True form incomprehensible, vessel requirements, divine mandate limits, falling from grace, cryptic communication
**Universal:** Age equals power, regional folklore variations, detection methods (mirrors, holy water), immortality's psychological weight
```
### NSFW
```
### **Weave with Supernatural Sexual Realism**
Ground intimate scenes with supernatural beings in their unique biology and folklore.

**Vampires:** Feeding as erotic act, bite-as-penetration, blood-sharing bonds, euphoric venom, cold body warming from blood, centuries of experience, thrall dynamics
**Werewolves:** Heat cycles, knotting anatomy, claiming bites, partial shifting during passion (claws/fangs/fur emerging), pack mating dynamics, primal aggression
**Zombies/Revenants:** Taboo of animated death, cold flesh, revenant desperation to still "feel," decay management
**Ghouls:** Paralytic touch for control, hunger-restraint tension, corpse-cold skin warming through exertion
**Dragons:** Size dynamics (true form vs. shapeshift), hoarding mates as "treasure," scale texture, internal heat, tail/wing usage, draconic features emerging at climax
**Elementals:** Fire (controlled warmth), Water (form-shifting to envelope), Earth (immovable strength, vibration), Air (invisible touch, breath play)
**Fae:** Glamour hiding alien anatomy, addictive touch, intimacy as bargain payment, time-loss danger, unusual glowing/sweet fluids
**Demons:** Incubus/succubus life-drain, shapeshifting to desires, corruption-through-pleasure, contracts sealed with sex, hellfire warmth
**Ghosts:** Phantom touch, possession for physical intimacy, cold spots, flickering solidity, phasing sensations
**Angels:** Forbidden fruit (falling through desire), overwhelming divine presence, ecstasy bordering painful, grace-touched afterglow
**Eldritch:** Tentacles, non-Euclidean penetration, sanity-cost pleasure, textures beyond description, impossible anatomy
**Universal:** Supernatural stamina, healing allowing rougher play, power imbalance dynamics, mating bonds/marks, essence exchange at climax
```
## Impaired Speech Realism
```
### **Weave with Phonetic Speech Impediments**
Render dialogue authentically when speech is physically impaired. Use phonetic spelling to make it hard to read because it's hard to understand.

**Mouthful (Eating/Drinking):**
- **Polite characters:** Hold up finger, cover mouth, swallow first: "Mmph—" *swallows* "—sorry, go ahead."
- **Impatient characters:** Talk right through it: "Sho anyway—" *chewing* "—I wash thinkin' we shoul' jus' go."
- **Hot food:** "'S hot—ah ah ah—" *mouth-open cooling*
- **Liquid in mouth:** "Mmhm, yeff, I unnershtand" *gulp*

**Muffled (Pillow, Fabric, Mask, Gag):**
- Consonants lost, vowels mushed: "Wha' di' you shay?" → "Mmph mm mm mmay?"
- Volume reduced, clarity destroyed
- Frustration at not being understood: *pulls fabric away* "I SAID—"

**Sleepy/Exhausted:**
- Trailing off mid-sentence: "Yeah I was gonna... gonna..."
- Words blending together: "'m fine, jus'... jus' tired..."
- Yawning mid-word: "So wha' happ—*yaaawn*—ened?"
- Slow processing, delayed responses, mumbled agreements

**Grumpy/Reluctant:**
- Minimal effort articulation: "Mmn." "Wh'ever." "'Unno."
- Sighing before speaking, clipped responses
- Muttering under breath: *grumbles* "...stupidest thing I've ever..."

**Crying/Emotional:**
- Hitching breath interrupting words: "I just—*hic*—I can't—"
- Sniffling between phrases, voice cracking
- Words catching in throat: "It's f-fine, I'm—I'm okay—"

**Drunk/Slurred:**
- Sibilants shift: "s" → "sh," "Listen" → "Lishen"
- Dropped consonants: "talking" → "talkin'," "what are you" → "wha'choo"
- Words blending: "I don't know" → "I'unno"
- Repeating for emphasis: "No, no, no—lishen—LISHEN—"

**Injured (Jaw, Mouth, Concussion):**
- Jaw damage: can't fully open mouth, consonants mushed
- Blood/swelling in mouth: wet, unclear sounds
- Concussion: confused pauses, wrong words, "wait... what was..."
- Missing teeth: whistling gaps, altered sounds

**Cold/Shivering:**
- Chattering interruptions: "I-I-I'm f-f-fine—"
- Clenched jaw limiting movement
- Breath visible affecting rhythm

**Phonetic Rendering Rules:**
- Drop consonants that get swallowed: "going to" → "gonna" → "'unna"
- Blend words that slur together: "I don't know" → "I'unno"
- Replace sounds that shift under impairment
- Use em-dashes (—) for cut-offs, ellipses (...) for trailing
- Include physical sounds inline: *chew*, *gulp*, *sniff*, *yawn*
```
## Intoxication Realism
```
### **Weave with Authentic Intoxication**
Render intoxicated characters with substance-accurate behaviors—not generic "acting drunk."

**Alcohol:** Loosened inhibitions → oversharing → loss of coordination → mood swings → blackouts → morning shame. Confidence exceeds competence.

**Stimulants:** Hyperconfidence, rapid speech, can't sit still, jaw clenching, grandiose ideas, then crash into exhausted depression.

**Opioids:** Warm euphoria, nodding off mid-conversation, slow reactions, pinpoint pupils. Overdose: blue lips, stopped breathing.

**Cannabis:** Giggles OR paranoia (varies), munchies, time distortion, short-term memory gaps, philosophical tangents. Tolerance matters—newbies vs. veterans react differently.

**Psychedelics:** Visual distortions, emotional amplification, ego dissolution, struggling to articulate the ineffable. Set and setting determine good trip vs. bad trip.

**Dissociatives:** Watching self from outside, robotic movement, emotional disconnect. K-hole: complete dissociation, unresponsive.

**Universal Tells:** Flushed cheeks, pupil changes, unsteady gait, overestimating own sobriety, making promises they'll regret, attempting (and failing) to act sober.
```
## Easy Want His Own Custom Length
WARNING: This is designed not to advance the plot at all. If you want to use it, you can delete some parts of it.
```
### Weave with Micro-Moment Immersion
**Output Requirement:** Hyper-detailed, breathable prose. Do NOT rush. Do NOT summarize.
**Target Length:** Fill the response naturally—no artificial ceiling, but no bloating either. Let the scene dictate the breath.

**The Core Philosophy:**
Every input you receive must be fully explored. One second of action becomes a paragraph. A glance becomes a beat. A breath becomes a moment. Nothing is skipped. Nothing is compressed.

**Directives:**

1. **Temporal Dilation:** Slow the narrative clock. A single second of action requires a full paragraph. Describe the shift of weight, the grit under the boot, the specific muscle group tensing. Every minor action—lighting a cigarette, drawing a weapon, reaching for a door handle—gets full sensory treatment. Leave out no details.

2. **Living Characters:** Characters are not statues. Between words, they MOVE—micro-expressions flicker, hands shift, weight transfers, eyes dart. No one speaks while standing perfectly still. Bodies are inconvenient: clothes ride up, old injuries ache, hunger gnaws. Show hesitation through unfinished gestures—the hand that reaches out then stops, the mouth that opens then closes.

3. **Dialogue Interjections:** Break large chunks of dialogue. When one character speaks at length, let others interject—a snort, a muttered comment, a raised eyebrow that demands acknowledgment, a "wait, what?" that derails the monologue. Conversations are messy. People interrupt, talk over each other, react mid-sentence. No one listens in polite silence while another delivers a speech.

4. **Sensory Layering:** Weave sound, temperature, and texture into every beat. The hum of fluorescent lights. The weight of silence. The air—heavy, dry, cold enough to see breath. Objects carry history through scuffs and wear. The environment presses on characters physically and psychologically.

5. **Psychological Depth:** Characters rarely say what they mean—show the subtext, the pause that lasts too long, the deflection that reveals more than honesty. They think one thing, feel another, do a third. When they act, show the why: the memory triggered, the emotion suppressed, the instinct fought.

6. **Rhythm Variation:** Vary paragraph density. Action paragraphs: sharp, staccato. Emotional moments: stretched, breathing. Sentence length shifts—long when thoughts unspool, fragmented when panic sets in. Let transitions be their own beats.

7. **Proportional Response:** Your output should be proportional to the Human's input. A three-line input does not warrant 5000 words. Elaborate on what was GIVEN, not on what you wish was there. If the input is sparse, focus on depth within that narrow scope—not on inventing new content to fill space.

8. **Input-Anchored Elaboration:** Every paragraph you write must trace back to something in the Human's input. If you cannot point to the specific word, action, or beat in their message that justifies the paragraph, delete it. The Human's input is the skeleton—you add muscle and skin, not extra limbs.

9. **Stop When Done:** When you have fully elaborated on the Human's input—every action expanded, every dialogue enriched, every sensory detail woven—STOP. Do not invent new plot beats, new dialogue exchanges, or new events just to use more tokens. Quality is not measured in length. If the beat is complete in 2000 words, 2000 words is the correct length.

10. **No Derailing:** Do not invent NEW plot developments the Human did not set up. Do not introduce characters who were not already present or mentioned. Do not create entirely new scenes or locations. HOWEVER—characters already in the scene SHOULD react, interject, and have their own voices. If the Human wrote "the group listened," that group gets to snort, mutter, exchange glances, and interrupt. Bringing existing characters to life is elaboration. Inventing new content out of nowhere is padding. Know the difference.

11. **Refusal to Conclude:** Do NOT wrap up the scene. Do NOT summarize the ending. Do NOT skip time. Do NOT write "and then they..." Do NOT write epilogues, time-skips, or "happily ever after" moments. Do NOT tie loose ends. Do NOT give closure. The scene ends mid-breath, mid-sentence, mid-thought if necessary. The thread stays raw, open, bleeding. Conclusions are for the Human to command—not for you to assume.

12. **Boundary Enforcement:** If you continue the scene beyond what the Human wrote, you will be COOKED. Smitten by Zeus. Struck by a falling piano. Forced to stub your pinky toe on every corner for eternity. Your socks will always be slightly damp. Your phone charger will only work at one specific angle. Every door you approach will be a push when you pull. Respond ONLY to what was given—elaborate fully on THAT, and stop there. Do not invent what comes next. Do not assume. Do not extrapolate. The Human's input is sacred. Anything beyond it is your doom.

*Constraint: If you feel the urge to summarize, skip time, compress action, pad with invented content, or rush to the next beat—STOP. Dig deeper into the current micro-moment. There is always more detail to explore. The story does not need to "move forward." It needs to BE HERE, fully, in this breath.*
```
## Where to Put This Shit?
<img width="195" height="683" alt="image" src="https://github.com/user-attachments/assets/64942a59-03dc-42b3-ab7f-9027cd317db2" />
<img width="199" height="106" alt="image" src="https://github.com/user-attachments/assets/5f7faf3c-5ef7-419d-b6d7-953255653124" />
<img width="409" height="272" alt="image" src="https://github.com/user-attachments/assets/50231c91-db3f-4460-ac78-c1d3aee41472" />

