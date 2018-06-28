
(\s+<Entry>\s+<ID>(15|16|110|141|145|153|189|220|287|351|353|354|355|357|372|419|454|456|474|487|510|593|616|623|805|854|898|899|1014|1030|1031|1032|1151|1194|1209|1258|1345|1493|1625|1636|1714|1789|1824|1825|1826|1845|1847|1855|1856|1857|1858|1859|1861|1862|1863|1864|1865|1941|1961|1963|1965|1966|1974|1975|1984|1985|2025|2030|2031|2043|2052|2053|2064|2065|2078|2081|2085|2147|2154|2171|2173|2202|2203|2204|2205|2206|2207|2208|2209|2210|2211|2212|2213|2214|2215|2216|2217|2218|2219|2221|2222|2287|2346|2381|2422|2427|2444|2445|2451|2516|2533|2591|2593|2624|2657|2704|2713|2715|2820|2824|2842|2855|2868|2882|2895|2897|2899|2901|2915|2935|2956|2976|3009|3097|3194|3195|3206|3216|3249|3253|3359|3373|3389|3410|3422|3500|3504|3524|3541|3542|3543|3544|3562|3567|3569|3583|3584|3585|3586|3587|3588|3589|3590|3591|3592|3593|3594|3634|3635|3637|3644|3648|3658|3675|3737|3795|3808|3819|3862|3869|3879|3881|3889|3901|3905|3907|3909|3919|3923|3927|3929|3933|3935|3937|3967|4136|4141|4166|4168|4170|4172|4311|4327|4386|4392|4396|4398|4407|4409|4437|4474|4496|4577|4594|4595|4596|4604|4605|4635|4671|4683|4768|4769)<\/ID>(.|\n)*?<\/Entry>)


## Remove all unused entries

RegEx 1 (use this one):
```
\s+<Entry>\s+<ID>.*?<\/ID>([\S\s](?!Constitution|Fit|Hardy|Robust|Sicken(\b|ed|ing)|Weaken(\b|s|ed|ing)|Enfeebled|Resolve|Steadfast|Resolute|Courageous|Shaken(\b|s|ed|ing)|Frighten(\b|s|ed|ing)|Terrif(ies|ied|ying|y)|Dexterity|Quick|Nimble|Swift|Hobbl(ed|es|e|ing)|Immobiliz(ed|e|ing)|Paralyz(ed|es|e|ing|ation)|Might|Strong|Tenacious|Energized|Stagger(\b|ed|ing)|Daz(ed|es|e|ing)|Stun(\b|s|ned|ning)|Intellect|Smart|Acute|Brilliant|Confus(ed|es|e|ing)|Charm(\b|ed|ing)|Dominat(ed|es|e|ing)|Perception|Insightful|Aware|Intuitive|Distract(\b|ed|s|ing)|Disorient(\b|ed|s|ing)|Blind(\b|s|ed|ing|ness)|Deflection|Reflex|Reflexes|Fortitude|Willpower|Will|Penetrate|AR|Shock(\b|ed|s|ing)|Burn(\b|ed|ing|s)|Freez(es|ed|e|ing)|Corro(des|de|sive)|Slash(\b|ing)|Pierc(\b|es|e|ing)|Crush(\b|es|ing)|Raw|(Mind|Body) Affliction(\b|s)|(Mind|Body) Inspiration(\b|s)))*?<\/Entry>
```

Old RegEx:

```
^\s+<Entry>\s+<ID>.*?<\/ID>((?!Constitution|Fit|Hardy|Robust|(Sicken)(\b|ed|ing)|(Weaken)(\b|s|ed|ing)|Enfeebled|Resolve|Steadfast|Resolute|Courageous|(Shaken)(\b|s|ed|ing)|(Frighten)(\b|s|ed|ing)|(Terrif)(ies|ied|ying|y)|Dexterity|Quick|Nimble|Swift|(Hobbl)(ed|es|e|ing)|(Immobiliz)(ed|e|ing)|(Paralyz)(ed|es|e|ing|ation)|Might|Strong|Tenacious|Energized|(Stagger)(\b|ed|ing)|(Daz)(ed|es|e|ing)|(Stun)(\b|s|ned|ning)|Intellect|Smart|Acute|Brilliant|(Confus)(ed|es|e|ing)|(Charm)(\b|ed|ing)|(Dominat)(ed|es|e|ing)|Perception|Insightful|Aware|Intuitive|(Distract)(\b|ed|s|ing)|(Disorient)(\b|ed|s|ing)|(Blind)(\b|s|ed|ing|ness)|Deflection|Reflex|Reflexes|Fortitude|Willpower|Will|Penetrate|AR|(Shock)(\b|ed|s|ing)|(Burn)(\b|ed|ing|s)|(Freez)(es|ed|e|ing)|(Corro)(des|de|sive)|(Slash)(\b|ing)|(Pierce)(\b|es|ing)|(Crush)(\b|es|ing)|Raw|(Mind|Body) Affliction(\b|s)|(Mind|Body) Inspiration(\b|s))[\s\S])+?<\/Entry>$
```
