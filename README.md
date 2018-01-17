# Slay The Spire - Brazilian Portuese Localization (Community)
Welcome, 
The project has just started. 

I'll update the `readme.md` with instructions as soon as i finish the configuration of the repository.

Please, be patient. 

> PS.: The Brazilian Portuguese files are in the `localization/ptb` folder.

---
## Oficial Translation Guide

Hello Slay the Spire translators! This is a helpful guide to try and aid your translation efforts.

1. As the files to translate are all JSON documents, fields do not need to be translated. In fact, the game won't run if the fields are renamed.
EXAMPLE: Only the fields under "NAMES" and "TEXT" needs to be translated. (Marked with <- This!)

```js
"Ironclad": {
    "NAMES": [
        "The Ironclad" <- This!
    ], 
"TEXT": [
        "The remaining soldier of the Ironclads. NL Sold his soul to harness demonic energies." <- This!
    ]
},
```

2. Formatting Quirks:
    -Text is colored to highlight keywords and other important concepts. Colors are as follows: #y, #r, #g, #b, #p. These colors are Gold, Red, Green, Blue, Purple (Only in events)
    EXAMPLE: "#yI'm #yGolden!"

    -For events and dialogs, if a word is surrounded by ~ or @, they are wavy or shaky in game. 
    EXAMPLE: "@This@ @is@ @shaky.@" "~This~ ~is~ ~wavy.~""

    -Colors and text effects can be combined. However, the color must always come before the effect.
    EXAMPLE: "#y@CLANG@ #y@CLANG@"

    -Cards utilize dynamic values. These are !D!, !B!, !M!. They stand for Damage, Block, and Misc.
    EXAMPLE: "Deal !D! damage."
    EXAMPLE: "Gain !B! Block."
    EXAMPLE2: "Draw !M! cards."

    -Keywords found in keywords.json must be capitalized when they are shown on a card, power, or relic description.
    EXAMPLE: "Apply 2 Vulnerable."

    -NL stands for new line. New lines are added to make the text feel easier to read or separates two distinct sentences or quotes. There must be a space on either side for the new line to be appended.
    EXAMPLE: "Hello. NL I am Bob."

    -Sometimes descriptions will be disjointed. This is because we need to insert dynamic values into some text.
    EXAMPLE:
    "I ate #b",
    " pies."
    Would look like: "I ate #b6 pies." in the game
	
3. Lore Quirks
    The animal references in Slay the Spire are misspelled because the animals aren't the same as the ones in our world, Earth- as the game doesn't take place anywhere near our time and place. Frog -> Phrog. Crane -> Krane. Bird -> Byrd are notable examples in the game.

4. If you have any questions, please reach out to us in the #localization channel on Discord. Don't forget to collaborate with others that are working on your language.

Thanks,
Anthony and Casey

---
## Oficial Updates 

### Updates for Translators!
----------------------------------

#### 1/15/2018:
- **ui.json**
  - New field "EXTRA_TEXT"
  -  Adding new field in "MenuButton"
  - Updated field Sounds in Background -> Ambient Sounds Effect in "OptionsPanel"
- **cards.json**
  - Added Upgrade Description for "Storm of Steel"

---

#### 12/12/2017 - 1/13/2018:
For Chinese (Traditional), German, French, Japanese, and Russian.
The following fields have been updated since the outsourced loc work. The files were sent out on  12/12/2017.

Sorry this one is so large! This is the first post in UPDATES.txt, future updates will be much smaller.

-  **achievements.json**
```
    "Best Win Streak: #y",
    "Highest Score: #y"
```

- **cards.json**
```
	Adrenaline
	Alchemize (ID is Venomology)
	Bandage Up
	Berserk
	Blind
	Bloodletting
	Bullet Time
	Calculated Gamble
	Clumsy
	Corpse Explosion
	Deep Breath
	Enlightenment
	Feed
	Flame Barrier
	J.A.X.
	Jack of All Trades
	Master of Strategy
	Mind Blast
	Nightmare
	Normality
	Offering
	Panacea
	Panache
	Purity
	Sadistic Nature
	Secret Technique
	Secret Weapon
	Transmutation
	Trip
```

- **characters.json**
```
	Neow
	"UNIQUE_REWARDS": [
		"[ #rLose #ryour #rstarting #rRelic. #gObtain #ga #grandom #gboss #gRelic. ]"
		"NeowsBlessing": {

	Neow Reward
	Before: "[ #gObtain #g3 #gPotions ]",
	After: "[ #gObtain #g3 #grandom #gPotions ]",
```

- **events.json**
```
	Accursed Blacksmith
	"[Locked] Requires: Upgradeable Cards"

	Bonfire Elementals
	"[Locked] Requires: Upgradeable Cards"

	Wheel of Change
	"[Locked] Requires: Upgradeable Cards"

	Mushrooms
	"[Locked] Requires: Upgradeable Cards"

	Winding Halls
	"[Focus] #rBecome #rCursed #r- #rWrithe. #gHeal #g",
```

-  **keywords.json**
```
	artifact was also added as a keyword
	format was updated so all fields must be re-translated
```

- **monsters.json**
```
    Cultist's Moves
   ```

- **potions.json**
```
    Elixir Potion
	"#yExhaust all #yStatus and #yCurse cards from your hand.",
   ```

- **powers.json**
```
	Nemesis
	"Reduce ALL damage taken and HP loss to #b1 for the next #b",
	" turn.",
	" turns."

	Nightmare (ID is Night Terror)
	"NAME": "Nightmare",
	"DESCRIPTIONS": [
	"At the start of your next turn, add #b",
	" cards to your hand."

	Envenom
	"Whenever you deal unblocked #yAttack damage, apply #b", 

	Minion
	"Minions abandon combat without their leader."

	Energized
	"Gain #b", 
	" additional [G] next turn."
	" additional [G] next turn.",
	" additional [G] next turn.",
	" - TRANSLATOR NOTE: - The above line is for plural if needed to distinguish from singular."

	Intangible
	" turns.",
	"Reduce ALL damage taken and HP loss to #b1 next turn."

	Painful Stabs
	"Whenever you take damage from this enemy, add a #yWound into your Discard Pile." 

	Split
	"When less than #b50% HP, will split into #b2 smaller slimes with ",
	"When its HP is at or below #b50%, will split into #b2 smaller slimes with ",

	Berserk
	"If your HP is at or below #b50%, gain ",

	Hex
	" #yDazed into your draw pile."
```
- **relics.json**
```
	Old Coin
	"Gain #b300 #yGold."

	The Courier
	"The merchant no longer runs out of cards, relics, or potions and his prices are reduced by #b20%."

	War Paint
	Darkstone Periapt
	Bottled Tornado

	Frozen Eye
	"When viewing your #yDraw #yPile, the cards are now shown in order."

	Juzu Bracelet
	"Regular enemy combats are no longer encountered in #y? rooms."

	Red Skull
	"While your HP is at or below #b50%, you have #b",

	Meat on the bone
	"If your HP is at or below #b50% at the end of combat, heal #b",

	Calling Bell
	"Skip Rewards",
	"Close"

	Neow's Lament
	"FLAVOR": "A blessing bestowed to you by Neow.",
    "DESCRIPTIONS": [
		"The first #b3 enemies you fight have only #b1 HP.",
		"The blessing is used up."

	Prayer Wheel
	"Non-Boss chests now also contain cards."

	Unceasing Top
	"Whenever you have no cards in hand during your turn, draw a card."

	Enchiridion
	"Start each combat with a random #yPower card in your hand. It costs #b0 until the end of turn."

	Cursed Key
	" Whenever you open a non-boss chest, obtain a #rCurse.",
```
- **tutorials.json**
```
	Draw tip
	" cards are drawn from here. NL NL Click to view the cards in your draw pile."

	Exhaust Tip
      "Click to view cards Exhausted this combat."
    "LABEL": [
      "Exhausted Cards"
    ]
```
- **ui.json**
```
	AbstractCard
	AbstractCreature
	AbstractMonster
	AbstractPlayer
	AbstractPotion
	ApplyPowerAction
	BattleStartEffect
	CampfireSleepEffect
	CampfireSmithEffect
	CampfireTokeEffect
	CampfireUI
	CharacterOption
	CombatRewardScreen
	CopyAction
	DiscardPileToTopOfDeckAction
	ExhaustAction
	ExhaustViewScreen
	ExhumeAction
	GameSavedEffect
	ImmolateAction
	LanguageDropdown
	LeaderboardFilters
	LeaderboardsScreen
	OpeningAction
	OptionsPanel
	PowerExpireTextEffect
	PutOnDeckAction
	RestartForChangesEffect
	RewardItem
	SingleCardViewPopup
	TipHelper
	UnlockTextEffect

	DrawPileViewScreen
				"(Cards shown are sorted alphabetically)",
```