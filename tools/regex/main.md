## Afflictions, inspirations + defensive and damage icon
```
(\s+<Entry>\s+<ID>.*?<\/ID>((?!((\b(Constitution|Fit|Hardy|Robust)\b)|((Sicken)(\b|ed|ing))|((Weaken)(\b|s|ed|ing))|((Enfeebl)(\b|ed))|(\b(Resolve|Steadfast|Resolute|Courageous)\b)|((Shaken)(\b|s|ed|ing))|((Frighten)(\b|s|ed|ing))|((Terrif)(\b|ies|ied|ying|y))|(\b(Dexterity|Quick|Nimble|Swift)\b)|((Hobbl)(|ed|es|e|ing)\b)|((Immobiliz)(|ed|e|ing)\b)|((Paralyz)(|ed|es|e|ing|ation))|(\b(Might|Strong|Tenacious|Energized)\b)|((Stagger)(\b|ed|ing))|((Daz)(\b|ed|es|e|ing))|((Stun)(\b|s|ned|ning))|(\b(Intellect|Smart|Acute|Brilliant)\b)|((Confus)(\b|ed|es|e|ing))|((Charm)(\b|ed|ing))|((Dominat)(\b|ed|es|e|ing))|(\b(Perception|Insightful|Aware|Intuitive)\b)|((Distract)(\b|ed|s|ing))|((Disorient)(\b|ed|s|ing))|((Blind)(\b|s|ed|ing|ness))|(\b(Deflection|Reflex|Reflexes|Fortitude|Willpower|Will|Penetrate|AR)\b)|((([sS]hock)(\b|ed|s|ing)\b)|(([bB]urn)(\b|ed|ing|s)\b)|(([fF]reez)(\b|es|ed|e|ing)\b)|(([cC]orro)(\b|des|de|sive)\b)|(([sS]lash)(\b|ing)\b)|(([pP]ierce)(\b|es|ing)\b)|(([cC]rush)(\b|es|ing)\b)|(Raw)\b)|(\b(Mind Afflictions)\b|\b(Body Afflictions)\b)))[0-9a-zA-Z,.&;'"#!-_+ <>\[\]\/\s\{\}\(\)\î\â])+?<\/Entry>)
```

### Alt version
```
^\s+<Entry>\s+<ID>.*?<\/ID>((?!(Constitution|Fit|Hardy|Robust|(Sicken)(\b|ed|ing)|(Weaken)(\b|s|ed|ing)|Enfeebled|Resolve|Steadfast|Resolute|Courageous|(Shaken)(\b|s|ed|ing)|(Frighten)(\b|s|ed|ing)|(Terrif)(ies|ied|ying|y)|Dexterity|Quick|Nimble|Swift|(Hobbl)(ed|es|e|ing)|(Immobiliz)(ed|e|ing)|(Paralyz)(ed|es|e|ing|ation)|Might|Strong|Tenacious|Energized|(Stagger)(\b|ed|ing)|(Daz)(ed|es|e|ing)|(Stun)(\b|s|ned|ning)|Intellect|Smart|Acute|Brilliant|(Confus)(ed|es|e|ing)|(Charm)(\b|ed|ing)|(Dominat)(ed|es|e|ing)|Perception|Insightful|Aware|Intuitive|(Distract)(\b|ed|s|ing)|(Disorient)(\b|ed|s|ing)|(Blind)(\b|s|ed|ing|ness)|Deflection|Reflex|Reflexes|Fortitude|Willpower|Will|Penetrate|AR|(Shock)(\b|ed|s|ing)|(Burn)(\b|ed|ing|s)|(Freez)(es|ed|e|ing)|(Corro)(des|de|sive)|(Slash)(\b|ing)|(Pierce)(\b|es|ing)|(Crush)(\b|es|ing)|Raw|(Mind|Body) Affliction(\b|s)|(Mind|Body) Inspiration(\b|s))\b)[\s\S])+?<\/Entry>$
```

## Afflictions, inspirations (no defensive and damage icons)
```
(\s+<Entry>\s+<ID>.*?<\/ID>((?!((\b(Constitution|Fit|Hardy|Robust)\b)|((Sicken)(\b|ed|ing))|((Weaken)(\b|s|ed|ing))|((Enfeebl)(\b|ed))|(\b(Resolve|Steadfast|Resolute|Courageous)\b)|((Shaken)(\b|s|ed|ing))|((Frighten)(\b|s|ed|ing))|((Terrif)(\b|ies|ied|ying|y))|(\b(Dexterity|Quick|Nimble|Swift)\b)|((Hobbl)(|ed|es|e|ing)\b)|((Immobiliz)(|ed|e|ing)\b)|((Paralyz)(|ed|es|e|ing|ation))|(\b(Might|Strong|Tenacious|Energized)\b)|((Stagger)(\b|ed|ing))|((Daz)(\b|ed|es|e|ing))|((Stun)(\b|s|ned|ning))|(\b(Intellect|Smart|Acute|Brilliant)\b)|((Confus)(\b|ed|es|e|ing))|((Charm)(\b|ed|ing))|((Dominat)(\b|ed|es|e|ing))|(\b(Perception|Insightful|Aware|Intuitive)\b)|((Distract)(\b|ed|s|ing))|((Disorient)(\b|ed|s|ing))|((Blind)(\b|s|ed|ing|ness))|(\b(Mind Afflictions)\b|\b(Body Afflictions)\b)))[0-9a-zA-Z,.&;'"#!-_+ <>\/\s])+?<\/Entry>)
```

## Mind and Body Afflictions

(\b(Mind Affliction)(\b|s)\b)

&lt;link="glossary://GlossaryEntry_Mind_Affliction"&gt;$1&lt;/link&gt;

(\b(Mind Inspiration)(\b|s)\b)

&lt;link="glossary://GlossaryEntry_Mind_Inspiration"&gt;$1&lt;/link&gt;

(\b(Body Affliction)(\b|s)\b)

&lt;link="glossary://GlossaryEntry_Body_Affliction"&gt;$1&lt;/link&gt;

(\b(Body Inspiration)(\b|s)\b)

&lt;link="glossary://GlossaryEntry_Body_Inspiration"&gt;$1&lt;/link&gt;


## Cyclopedia touch-ups
```
&lt;link="glossary:\/\/GlossaryEntry_(Inspirations|Afflictions)_(Perception|Constitution|Dexterity|Might|Resolve|Intellect)"&gt;&lt;#(00a4ff|ff4800|ca58ff|f7b733|72da26|30d3d5)&gt;(Perception|Constitution|Dexterity|Might|Resolve|Intellect)&#160;(Affliction|Afflictions|Inspiration|Inspirations)&#160;&lt;\/color&gt;&lt;\/link&gt;\.
```

```
&lt;size=80%&gt;&lt;link="glossary://GlossaryEntry_$1_$2"&gt;&lt;#dac79c&gt;$4&#160;$5&#160;&lt;/color&gt;&lt;/link&gt;.&lt;/size&gt;

```

```
&lt;link="glossary:\/\/GlossaryEntry_(Piercing|Slashing|Crushing|Raw|Burning|Corrode|Freezing|Shock)"&gt;(([sS]hock)(\b|ed|s|ing)|([bB]urn)(\b|ed|ing|s)|([fF]reez)(\b|es|ed|e|ing)|([cC]orro)(\b|des|de|sive)|([sS]lash)(\b|ing)|([pP]ierce)(\b|es|ing)|([cC]rush)(\b|es|ing)|(Raw)\b)&lt;space=0.7em&gt;&lt;sprite="Inline" name="cs_(pierce|slash|blunt|raw|burn|corrosive|freeze|schock)" tint=1&gt;&lt;space=0.7em&gt;Damage&lt;\/link&gt;
```

```
&lt;link="glossary://GlossaryEntry_$1"&gt;&lt;b&gt;$2&lt;/b&gt;&lt;space=0.7em&gt;&lt;sprite="Inline" name="cs_$3" tint=1&gt;&lt;/link&gt;&lt;space=0.7em&gt;damage
```


## Cyclopedia 2.0
```
&lt;link="glossary:\/\/GlossaryEntry_([A-Za-z]*?)_([a-zA-Z]*?)"&gt;&lt;#(\w*?)&gt;([a-zA-z]*?)&#160;([a-zA-Z]*?)&#160;&lt;sprite="Inline" name="attribute_([a-z]*?)" tint=1&gt;&lt;\/color&gt;&lt;\/link&gt;\.
```
Replace with:
```
&lt;size=80%&gt;&lt;link="glossary://GlossaryEntry_$1_$2"&gt;&lt;#dac79c&gt;$4&#160;$5&lt;/color&gt;&lt;/link&gt;&lt;/size&gt;

```
```
&lt;size=80%&gt;&lt;link="glossary:\/\/GlossaryEntry_([A-Za-z]*?)_([A-Za-z]*?)"&gt;&lt;#dac79c&gt;([A-Za-z]*?)&#160;([A-Za-z]*?)&#160;&lt;\/color&gt;&lt;\/link&gt;&lt;\/size&gt;
.&
```
