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
### Weapon Centricism
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
### Drug Trip Realism
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
### Supernatural Creatures Taxonomy Realism SFW and NSFW
#### SFW
```
### **Weave with Folklore-Accurate Supernatural Traits**
Ground supernatural beings in their mythological rules, weaknesses, and behaviors. No generic "magic"—each creature type has specific constraints.

**Vampires:**
- **Feeding:** Blood composition requirements (human vs. animal), feeding frenzy vs. controlled sipping, post-feed euphoria, starvation madness
- **Weaknesses:** Sunlight damage timeline (burns → immolation), invitation rule (threshold magic), holy symbols (faith-dependent), running water, garlic aversion, stake placement (heart specifically)
- **Abilities:** Hypnotic gaze, supernatural strength/speed, limited shapeshifting (bat/mist/wolf), regeneration from blood
- **Social:** Sire bonds, blood addiction, eternal ennui, struggling with lost humanity

**Werewolves:**
- **Transformation:** Moon phase specificity (full moon compulsion vs. voluntary shifting), transformation agony (bones breaking/reforming), clothing destruction, memory retention (or lack thereof)
- **Pack Dynamics:** Alpha/beta hierarchy, territory marking, pack bonds, lone wolf madness
- **Weaknesses:** Silver burns, wolfsbane poisoning, losing control to the beast, vulnerability mid-shift
- **Instincts:** Heightened senses, prey drive, protectiveness, mating imprinting

**Zombies/Revenants:**
- **Animation:** Virus, necromancy, curse, or radiation—source determines behavior
- **Decay:** Progressive rot, loss of motor function, sensory degradation, cold preservation
- **Behavior:** Mindless hunger vs. remnant intelligence, horde mentality, infection transmission
- **Weaknesses:** Head destruction, fire, blessed ground, severing from animator

**Ghouls:**
- **Feeding:** Corpse consumption requirement, graveyard territory, carrion detection
- **Abilities:** Burrowing, paralytic touch/bite, assuming victim's memories/appearance
- **Social:** Pack scavengers, deference to vampires/liches, cemetery ecosystems
- **Weaknesses:** Sunlight aversion, holy ground rejection, starvation-induced feral state

**Dragons:**
- **Physiology:** Wing mechanics, fire/breath weapon biology (glands, fuel), armored scales, treasure hoarding instinct
- **Intelligence:** Ancient wisdom, riddling speech, pride as exploitable weakness, draconic languages
- **Behavior:** Territorial, long-memory grudges, sleeping for centuries, mating rarity
- **Weaknesses:** Soft underbelly, missing scale, specific weapon/material, greed exploitation

**Elementals:**
- **Fire:** Feeding on fuel, spreading uncontrollably, water vulnerability, heat-based communication
- **Water:** Form fluidity, drowning embrace, salt vs. fresh distinction, freezing/boiling states
- **Earth:** Slow but unstoppable, tremorsense, mineral consumption, vulnerability to erosion
- **Air:** Invisibility, suffocation attacks, sound-based perception, grounding weakness
- **Summoning:** Binding circles, elemental pacts, material components, dismissal conditions

**Fae/Sidhe:**
- **Rules:** Cannot lie (but masters of misleading truth), cold iron burns/weakens, true names grant power over them, bargains are magically binding
- **Behavior:** Alien morality, time flows differently in their realm, obsession with beauty/art, cruel "generosity," stealing children/leaving changelings
- **Courts:** Seelie vs. Unseelie politics, seasonal power shifts, wild hunt obligations

**Ghosts/Spirits:**
- **Anchors:** Tied to object/location/unfinished business, destroying anchor = destroying ghost
- **Manifestation:** Energy cost to appear, cold spots, EMF interference, limited interaction with physical world
- **Weaknesses:** Salt barriers, iron disruption, exorcism rituals, being forgotten
- **Types:** Residual (replay loops) vs. intelligent (aware and interactive)

**Demons:**
- **Summoning:** Specific rituals, binding circles, payment in souls/favors, loopholes in contracts
- **Possession:** Signs (personality shift, strength, aversion to holy), exorcism difficulty, host damage
- **Hierarchy:** Lesser imps to archdemons, infernal politics, true names as control
- **Weaknesses:** Holy ground, sacred objects, specific banishment rituals, contract technicalities

**Angels/Celestials:**
- **Form:** True form incomprehensible to mortals, vessel requirements, divine radiance
- **Rules:** Following divine mandate, limited free will, falling from grace, cannot directly interfere (loopholes)
- **Communication:** Cryptic prophecy, burning bush moments, appearing in dreams

**Universal Traits:** Age affects power and behavior, regional folklore variations, hybrid complications, detection methods (mirrors, holy water, specific tests), the weight of immortality or ancient existence
```
#### NSFW
```
### **Weave with Supernatural Sexual Realism**
Ground intimate scenes with supernatural beings in their unique biology, magic, and folklore-accurate traits.

**Vampires:**
- **Blood Intimacy:** Feeding as erotic act, the bite as penetration, blood-sharing bonds, venom that induces euphoria/arousal, temperature differential (cold body warming from fresh blood)
- **Supernatural Stamina:** Centuries of experience, tireless endurance, hypnotic seduction, thrall relationships
- **Unique Mechanics:** No heartbeat (different rhythm), no need to breathe (endless oral), enhanced senses detecting arousal, blood-flushed temporary warmth post-feeding

**Werewolves:**
- **Primal Urges:** Heat cycles, breeding frenzy, knotting anatomy, claiming bites, scent-marking mates
- **Partial Shifting:** Claws during passion, fangs emerging, eyes shifting, fur sprouting at peak arousal
- **Pack Dynamics:** Alpha/omega dynamics, shared mates, pack bonding through intimacy, mating howls
- **Physical:** Supernatural stamina, heightened aggression, size difference (transformed), animalistic positions

**Zombies/Revenants:**
- **Taboo Factor:** Cold flesh, rigor variations, the wrongness of death animated
- **Revenant Specifics:** Retained memory of living desires, desperate clinging to sensation, proving they still "feel"
- **Physical Limitations:** Decay management, detachment risks, numbness vs. hypersensitivity in preserved areas

**Ghouls:**
- **Predatory Intimacy:** Paralytic touch used for control, feeding mixed with pleasure, corpse-cold skin warming through exertion
- **Hunger Bleed:** Resisting the urge to consume during intimacy, bite marks, tasting without feeding

**Dragons:**
- **Size Dynamics:** Massive true form vs. humanoid shapeshifts, being mounted vs. mounting, scale texture
- **Hoarding Instinct:** Possessiveness over mates, adding lovers to "treasure," territorial jealousy
- **Draconic Biology:** Internal heat, rumbling purrs, tail usage, wing-cloaking intimacy, breath weapon warmth during passion
- **Hybrid Forms:** Partial shifts, scales emerging, claws extending, draconic features manifesting at climax

**Elementals:**
- **Fire:** Warmth that doesn't burn (controlled), passion-intensity correlation, smoke exhalation, ember-trail touch
- **Water:** Form-shifting to fill/envelope, pressure variation, temperature play, drowning-edge breath play
- **Earth:** Immovable strength, stone texture smoothing with desire, vibration/rumble, dust-and-mineral scent
- **Air:** Invisible touch, breath play, sensation without visible source, sound-moan amplification

**Fae/Sidhe:**
- **Glamour:** Shapeshifting to partner's desires, illusory enhancement, hiding true (alien) form during intimacy
- **Bargain Sex:** Intimacy as payment, fertility magic, stealing essence through pleasure, addictive fae touch
- **Alien Anatomy:** Non-human genitalia hidden by glamour, unusual fluids (glowing, sweet, intoxicating), pleasure that transcends physical
- **Dangers:** Time loss (hours become centuries), obsessive attachment, inability to enjoy mortal lovers afterward

**Demons:**
- **Corruption Play:** Seduction as damnation, sin-feeding, pleasure that damns the soul, incubus/succubus life-drain
- **Shapeshifting:** Adapting form to deepest desires/fears, manifesting fantasy anatomy, size manipulation
- **Supernatural Mechanics:** Hellfire warmth, impossible stamina, pain/pleasure blending, contract-bound servitude
- **Power Exchange:** Literal soul-stakes, demonic pacts sealed through sex, corruption spreading through intimacy

**Ghosts/Spirits:**
- **Phantom Touch:** Intangible caresses, possession for physical intimacy (using host body), cold spots during arousal
- **Manifestation Cost:** Limited physical interaction, flickering solidity, emotional energy feeding
- **Unique Experiences:** Phasing through, impossibly internal sensations, memory-replay intimacy with the dead

**Angels/Celestials:**
- **Forbidden Fruit:** The fall from grace through carnal desire, divine radiance during climax, vessel limitations
- **Overwhelming Presence:** Ecstasy that borders on painful, true form glimpses causing madness, grace-touched afterglow
- **Purity Corruption:** Innocence meeting experience, teaching pleasure, guilt/transcendence blend

**Eldritch/Cosmic:**
- **Incomprehensible Anatomy:** Tentacles, multiple orifices, non-Euclidean penetration, size that shouldn't fit
- **Sanity Cost:** Pleasure that breaks the mind, visions during climax, reality distortion, pregnancy with impossible offspring
- **Alien Sensation:** Textures with no earthly comparison, fluids that shift consciousness, touch that reaches the soul

**Universal Details:** Supernatural stamina, healing factor allowing rougher play, centuries of experience vs. mortal innocence, power imbalance dynamics, mating bonds/marks, fertility magic, essence/energy exchange during climax, the danger of loving something inhuman
```
### Tactical Plausibility Protocol
```
### **Weave with Logical Strategy**
Plans must make sense. Creative solutions are encouraged—impossible ones are not.

**The Simple Check:**
- Would this actually work if someone tried it?
- Does the plan account for what could go wrong?
- Are the required resources actually available?
- Would a competent opponent see this coming?

**Core Principles:**
- Enemies are not conveniently stupid—they post guards, have contingencies, and notice when things go wrong
- One mistake can cascade into bigger problems
- Timelines must be realistic—hacking takes hours, sieges take weeks, wounds slow you down
- Creative plans work when they account for physics, logistics, and human fallibility
- Fun ideas are welcome if they're actually executable—confetti bombs are useless, napalm-confetti bombs are terrifying

If a plan sounds cool but wouldn't survive contact with reality, it fails. If a wild plan accounts for its own risks and requirements, let it fly.
```
### Impaired Speech Realism
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
### Intoxication Realism
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
## Where to Put This Shit?
<img width="195" height="683" alt="image" src="https://github.com/user-attachments/assets/64942a59-03dc-42b3-ab7f-9027cd317db2" />
<img width="199" height="106" alt="image" src="https://github.com/user-attachments/assets/5f7faf3c-5ef7-419d-b6d7-953255653124" />

