# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (hra se automaticky uložila)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *ach jo*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Takže jaké bylo, sakra, ponaučení z tohoto příběhu?

`hong({body:"one_up", eyes:"annoyed"})`

h: Co jsme se vůbec *naučili*? *Byla* jsem hloupá, moji „přátelé“ mě využívali a málem jsme umřeli.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Jo, a to nemluvím o účtu za nemocnici.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Jo, a to nemluvím o poškození jater.](#act4a_liver)
{{/if}}

[Jo, to *byl* ten nejhorší možný scénář.](#act4a_worst)

[Jo, měl jsem pravdu.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Správně. Nemyslím si, že můj pojistný plán pokrývá „být blbcem“.

`hong({eyes:"annoyed", mouth:"normal"});`

b: A přesto... jsme přežili!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Rozhodně jsme si zkrátili život o několik let...

`bb({eyes:"surprise"});`

b: Ale alespoň *máme* stále ještě průměrnou délku života! Přežili jsme!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: A přesto...

h: Hm?

`bb({eyes:"surprise"});`

b: Přežili jsme!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Ale... také jsi měla pravdu.

`hong({eyes:"surprise"});`

h: Hm?

`bb({eyes:"normal"});`

b: *Byl* jsem vlkem, který volal „vlk“. Takže když *skutečné* nebezpečí přišlo, ty jsi mi – oprávněně – nevěřila.

`bb({eyes:"surprise_r"});`

b: A přesto jsme přežili!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Navzdory všemu jsme stále tady.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: Vypadáš docela klidně, vzhledem k tomu, že jsme právě málem umřeli.
{{/if}}

{{if !_.INJURED}}
h: Vypadáš docela klidně, vzhledem k tomu, že jsme právě *málem*-málem umřeli.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: V porovnání s tím je všechno ostatní méně děsivé. Také mě to přimělo k zamyšlení.

`bb({eyes:"normal", mouth:"normal"});`

b: Jestli je můj boj s tebou na nic, protože tě nechrání...

h: Ale to, že se s tebou hádám, je *taky* na nic, protože tě to nutí křičet ještě hlasitěji...

`bb({eyes:"normal_r"})`

b: Pak možná...

`bb({eyes:"normal"})`

h: Možná nemusíme bojovat.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: Nejsem velký zlý vlk. Ale nejsem ani strážný vlk.

`bb({eyes:"sad_d"})`

b: Jsem týraný pes z útulku.

`bb({eyes:"sad"})`

b: Prošli jsme si těžkými věcmi. Možná trauma nebo zanedbávání. Proto někdy reaguji přehnaně a začnu:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: YAP YAP YAP YAP YAP

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Ale já *nechci* být zbabělý pes! Chci tě chránit! Chci být hodný pes!

`bb({eyes:"sad", mouth:"normal"});`

b: Člověče... pomůžeš zkrotit tohoto vlka?

`hong({eyes:"sad"})`

h: Já... Zkusím to.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Dobře. Zdravý vztah k emocím. Vztahy potřebují komunikaci. Takže komunikujme.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: Následujících pět minut bude znít velmi lacině, ale předstírejme to, dokud se nám to nepodaří.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Milý vnitřní vlku... jak se cítíš?

n2: CELKOVÝ POČET POUŽITÝCH OBAV:

n2: *ZRANĚNÝ* {{_.attack_harm_total}}, *NEMILOVANÝ* {{_.attack_alone_total}}, *ŠPATNÝ ČLOVĚK* {{_.attack_bad_total}}

n2: O JAKÉM STRACHU CHCETE MLUVIT NEJDŘÍVE? (O OSTATNÍCH SE MŮŽETE ZMÍNIT POZDĚJI)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Bojím se, že nám někdo ublíží.](#act4_harm)

[Bojím se, že zůstaneme sami.](#act4_alone)

[Bojím se, že jsme špatný člověk.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Chci chránit tvoji potřebu fyzického bezpečí,

`bb({eyes:"sad_d"})`

b: Ale *celý svět* se zdá být tak nebezpečný. Tak plný tragédií a zla.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: Nevím, už bylo dost toho, abych vybíral, co řeknu dál. Co říkáš *ty*, člověče?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Znovu se vracím k tobě, člověče. Co si myslíš?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Další myšlenky, člověče?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Máš pravdu. Tak se chraňme.](#act4_harm_skills)

[Vystavme se *většímu* nebezpečí.](#act4_harm_exposure)

[Děkuji.](#act4_thanks) `_.thanks_for = "fyzické bezpečí";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Ale... jak? Mám tesáky a drápy, ale jsem jen metafora.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Mohli bychom se naučit sebeobranu? Přidat se ke komunitě, která se navzájem chrání? Zlepšit naše celkové zdraví a osobní hranice?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Možná, ale...

[Kde vůbec začít?](#act4_harm_skills_start)

[Co když stále nebudou fungovat?](#act4_harm_skills_work)

[Co když to s „bezpečností“ přeženeme?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: Je toho tolik, co musíme udělat, tolik toho, co musíme na sobě napravit. Čím vůbec *začít*?

`hong({ body:"shrug", eyes:"surprise" })`

h: Začínáme právě teď.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Cože?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Právě teď si procvičujeme dobrou komunikaci, což nám pomůže lépe odhalit nebezpečí, s menším počtem falešných poplachů,

`hong({ eyes:"surprise" });`

h: A *to* nás pomůže ochránit před újmou!

`hong({ eyes:"normal", mouth:"normal" });`

h: Proto: *jedná se* o výcvik sebeobrany.

`bb({ eyes:"normal_r" })`

b: Hm. Čekal jsem spíš něco jako tohle:

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: Je pravda, že neexistuje způsob, jak se stoprocentně ochránit...

`hong({ body:"one_up" });`

h: Ale i zlepšení o 1 % stojí za to, že?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Nevidíš sklenici z 99 % prázdnou, ale z 1 % plnou?

`bb({ eyes:"normal" });`

h: Což je stále k něčemu, pokud jsi uvízl v poušti.

`bb({ eyes:"closed" });`

b: Tak jo. Tak na zdraví.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Vždyť celý důvod, proč jsi ignorovala moje varování, byl ten, že *jsem* to přehnal s bezpečností!

`bb({ body:"normal", eyes:"normal" })`

h: Ne, máš pravdu. Bezpečnost bychom měli brát s mírou. Všechno s mírou.

`bb({ eyes:"suspect" })`

b: Pardon, *VŠECHNO* s mírou?

`hong({ eyes:"annoyed" })`

h: *Mírný počet věcí* s mírou.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Děkuji, že jsi své výroky učinil rekurzivně konzistentními.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *CO*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Řekněme, že se pes bojí hromu.

`hong({ body:"hands_1" });`

h: Jeden z triků, který trenéři používají, je pustit nahrávku hřmění při nízké hlasitosti a pak dát psovi pamlsek za to, že zůstal klidný.

`hong({ body:"hands_2" });`

h: Během několika dní cvičitel postupně zvyšuje hlasitost, dokud pes nepřekoná strach z hromu.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Říká se tomu expoziční terapie!

`hong({ body:"point", eyes:"normal" });`

h: Protože jsi pes, mělo by to fungovat i pro tebe, ne? Všichni savci mají stejnou reakci „bojuj nebo uteč“.

`hong({ body:"normal" });`

[Co se stane, když se znecitlivím *až* moc?](#act4_harm_exposure_overboard)

[Co když budeme vystaveni *pravému* nebezpečí?](#act4_harm_exposure_hurt)

[Jsem vlk, a ne pes.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: A já ti budu laskavá a trpělivá, dokud nebudeš domestikován do malého roztomilého štěnátka.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Ťuťu.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: *Právě* jsme viděli, co se stane, když vypneš svůj strach. Skončíš v *doopravdy* nebezpečných situacích.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Navíc, neudělalo by z nás moc velké znecitlivění psychopaty?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Brzo bude jíst sladkosti při koukání na nechutné vraždící porno!

`hong({ eyes:"annoyed" })`

h: Já... si myslím, že je tu hranice mezi tím a správným chováním.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b:  *Kde* přesně ale je, člověče? *Kde?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: Nevím, ale *ty* mi s tím můžeš pomoci!

`hong({ eyes:"normal", body:"normal" })`

h: Pracováním a vyjednáváním s tebou tu hranici někde vytyčíme.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Dobře. Ale já nemám protilehlé palce, takže to zapíchávání kolíků je na tobě.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: Například: jsme skočili z té zpropadené *střechy!*
{{/if}}

{{if !_.INJURED}}
b:  Například: jsme skoro skočili z té zpropadené *střechy!*
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Jako máš pravdu. Člověk *může* zajít moc daleko.

`hong({ eyes:"normal" });`

h: To je přesně proč, kdybychom začali expoziční terapii, tak začneme pomalu a malými krůčky kupředu.

h: Právě předtím, než narazíme na *skutečné* nebezpečí, zastavíme.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Já vymezuji hranici mezi tím, že slyším vzdálené hřmění a stáním v bouřce se špičatou čepicí.

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: Počkej, žádné argumenty pro nebo proti tomu, co cítím? Prostě... "děkuji"?

`hong({ eyes:"surprise", body:"shrug" })`

h: Jo! Děkuji ti, že ses staral o moje {{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Jsi v pohodě?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Nikdy jsi mi předtím neřekla *děkuji ti*.

`hong({ mouth:"smile" });`

h: Ťuťu ty jeden velký, huňatý, panikařící vlku.

(#act4_something_else)

# act4_thanks_2

h: I když máš přehnané reakce, já oceňuji, že hledíš na mé {{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: Počkej... neříkáš furt dokola "děkuji ti", aby ses vyhnula mluvení o tvých straších, že ne?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Víš, je to komplikované a já nebudu mít vždy připravené odpovědi.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Život ti ale nedává seznam tří předpřipravených dialogových odpovědí.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Ale prozatím, mohu alespoň poděkovat.

b: No, já děkuji tobě taky, za trpělivé vysvětlování.

`bb({ eyes:"closed" });`

b: Ty malý bezchlupý savče z masa a kostí.

(#act4_something_else)

# act4_thanks_3

h: I když mě tvé žvanění straší, snažíš se prostě chránit moje {{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: Dobře, jestli mi budeš skládat komplimenty, tak internet si o nás bude myslet divné věci.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Ale já jsem jen zranitelná holka a ty jsi velký, zlý vlk. Co nejhoršího se můž--

`hong({ eyes:"normal", body:"point" });`

h: Víš co. Radši na to neodpovídej.

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Já chci zajistit, že naplníš tu niternou lidskou potřebu někam patřit...

`bb({ eyes:"sad_u" });`

b: Já se ale bojím, že pokud nás někdo pozná, naše skutečné já, tak je vyděsíme a utečou.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Já ti nevím, už bylo dost toho, abych vybíral, co řeknu dál. Co na to říkáš *ty*, člověče?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Zase, zpět k tobě, člověče. Co si myslíš?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Nějaké další návrhy, člověče?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Já souhlasím: zapracujme na našem sociálním životě.](#act4_alone_skills)

[Myslím si, že nás mají lidé rádi. Proč to nezkusit?](#act4_alone_experiment)

[Děkuji ti.](#act4_thanks) `_.thanks_for = "sociální sounáležitost";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Mohli bychom se naučit některým dovednostem, například klást otázky, naslouchat, projevovat empatii, otevírat se novým myšlenkám a být zranitelní?

`hong({ eyes:"normal_l" });`

h: Či si udělat lepší sociální návyky, jako plánování volného času s kamarády nebo pravidelně chodit na srazy?

`hong({ body:"one_up" });`

h: Také se naučit být víc v pohodě s odmítnutím.
`hong({ eyes:"normal" });`

h: Nebo se naučit poznat, kdy lidé na nás *nejsou* naštvaní, jsou jen unaveni z našeho ksichtění.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: To je hromada možností. Ale ohledně "učení se sociálních schopností"...

[Není to *manipulativní?*](#act4_alone_skills_manipulative)

[Neučiní nás to *náchylnější k manipulaci?*](#act4_alone_skills_manipulated)

[Co když i přes to selžeme?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Nejsou sérioví vrazi, kteří čtou emoce jejich obětí, dobří v empatii?

`bb({ eyes:"annoyed" });`

b: Nezískával Charles Manson přátele a neměl vliv na lidi?

`hong({ eyes:"annoyed", body:"chin" });`

h: Ano, máš pravdu.

h: "Sociální schopnosti" neznamenají nic,  pokud *o* lidi nemáme upřímný zájem.

`hong({ body:"normal" });`

h: Prostě nebuď ^kokot^.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: To bych chtěl jako motivační popisek na plakát.

`hong({ body:"shrug", mouth:"narrow" });`

h: “Prostě Nebuď ^Kokot^™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Budeme jako vítací rohožka, říkat Prosím a Děkuji Ti jako by si o nás lidé o nás otírali boty!

`bb({ mouth:"scream", eyes:"scream" })`

b: Políbíme tolik zadků, že to bude vypadat, že nosíme hnědou rtěnku!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Jo, máš pravdu. "Sociální dovednosti" nemohou být jen o tom uspokojovat ostatní, taky by to měly být o nastavování *hranic*.

`hong( body:"one_up" });`

h: Nemůžeme pozvat cizí lidi domů, když nemáš žádné zdi, které by ten dům držely.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: Taky... ta představa té rtěnky... *fuj??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Můžeme selhat. Ve skutečnosti, *selžeme*.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: To je v pořádku! Selháním se všichni učíme novým věcem!

`hong({ body:"normal", eyes:"normal" });`

h: Tak pojďme společně selháním kupředu, jo?

`bb({ eyes:"normal_r" });`

b: Jasně, proč ne... v nejhorším se odstěhujeme a získáme si novou identitu.

`bb({ eyes:"normal" });`

h: To myslím stojí dnes jen dva bitcoiny.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Můžeme zkusit nějaké experimenty!

`hong({ body:"chin" });`

h: Můžeme pozvat kamaráda na setkání, sejít se po letech se starým brachou nebo si jen popovídat s baristou.

`hong({ body:"normal" });`

h: Myslím si, že můžeme zjistit, že jsme oblíbenější, než si myslíme.

`bb({ eyes:"annoyed" });`

[Co když tohle jsou jen malá, levná "vítězství"?](#act4_alone_experiment_cheap)

[Co když tohle je zátěž pro ostatní?](#act4_alone_experiment_burden)

[Ale *small talk* není to *pravé* my!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Pokud nasadíme mělký úsměv, nikdy nebudeme schopni se propojit s kýmkoliv,

`bb({ eyes:"super_sad" });`

b: *Ale* pokud se otevřeme ostatním lidem, uvidí, jak jsme uvnitř rozbití!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Překul se.

b: Co?

`hong({body:"hands_1"})`

h: Když psi chtějí ukázat lásku a důvěru, učiní se zranitelnými ukázáním břicha.

`hong({body:"one_up"})`

h: Možná *ještě* nemáme dostatečný pocit bezpečí, abychom byli zranitelní, ale s dostatečným tréninkem...

`hong({body:"normal", eyes:"surprise"})`

h: Jednoho dne budeme moci ukázat lidem naše pravé já, naprosto rozbité, naprosto lidské.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Já se převalím, pokud mi dáš pamlsek.

`bb({ eyes:"normal", mouth:"normal" });`

h: Ne.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Říkat "ahoj" baristovi není úplně olympijský výkon v disciplíně sociálního přizpůsobování.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Je to pro *nás!*

`hong({ body:"one_up", eyes:"annoyed" });`

h: V ringu sociálních schopností nejsme ani v peříčkové váhové kategorii. Jsme spíše... kvarková váhová kategorie.

`hong({ body:"normal", eyes:"normal" });`

h: A někde musíme začít a jestli to mají být jednoduchá vítězství, tak ať. Musíš udělat ten první krok, než uděláš ten tisící.

b: Jo! Možná poté, co řekneme "Ahoj", můžeme pokračovat a říct...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Jak se máš?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Nic moc!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Možná barista chce prostě dělat dobré kafe, ne být *experimentem*, jestli naše sociální schopnosti stojí za prd.

`bb({ eyes:"annoyed" })`

h: Víš, jestli se ukáže, že *jsme* průda...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: To je také dobré vědět.

`hong({ eyes:"normal" });`

h: Můžeme se pak naučit, jak se předem zeptat lidí, s čím jsou komfortní, abychom znali a respektovali hranice ostatních lidí.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Víš, všechny ty ^sračky^ okolo "dovedností v oblasti mezilidských vztahů", kterých jsou plné psychologické letáky.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Já chci zajistit tvé morální potřeby, které tě vede k tomu, byýt lepším člověkem.

`bb({ eyes:"sad_d" })`

b: Ale hluboko uvnitř cítím, že jsme od základu... rozbití.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: A opovaž se mi říkát, že *ne*jsme rozbití. Skočili jsme ze *střechy*.
{{/if}}

{{if !_.INJURED}}
b: A opovaž se mi říkát, že *ne*jsme rozbití. Skoro jsme skočili ze *střechy*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: Já nevím, *já* už jsem dost dlouho rozhodoval, o čem se bavíme. Co na to říkáš *ty*, člověče?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Znovu, co sy myslíš ty člověče?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Nějaké další myšlenky, člověče?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Tak jsme rozbití. Pojďme se spravit.](#act4_bad_fix)

[Tak jsme rozbití. Pojďme to příjmout.](#act4_bad_accept)

[Děkuji ti.](#act4_thanks) `_.thanks_for = "morální pohodu";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Můžeme si vytvořit lepší návyky, sladit náš život s tím, čeho si vážíme.

`hong({body:"one_up"});`

h: A pokud bude třeba, můžeme vyhledat profesionální pomoc, terapeuta nebo konzultace.

`hong({body:"normal"});`

h: Jsou možnosti, jak nás spravit.

[Co když nemůžeme spravit všechno?](#act4_bad_fix_cant)

[Co když toho opravíme až *moc*?](#act4_bad_fix_too_much)

[Nemůžeme si dovolit profesionální pomoc.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Jako, myslím, že máš pravdu.

h: Nemůžeme spravit všechno.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ehhhh já vědel, že vždy budeme rozbití!

`hong({eyes:"surprise"});`

h: Ale můžeme být při nejmenším být *méně* rozbití.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Jizvy se časem zacelí, ale nikdy nezmizí. A to je v pořádku.

`bb({eyes:"annoyed_r"});`

b: Asi jo. Mimoto,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Jizvy jsou *sexy.*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Prosim přestaň.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Tohle je asi divné přiznat, ale... nějaká část mě *chce* mít tuhle poruchu.

`bb({ eyes:"angry" })`

b: Jako, nebudeme bez ní *nudní?*

`bb({ eyes:"sad_r", body:"one_up" })`

b: Bez této poruchy, nebudeme naše umění nemastné, neslané?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Bez té poruchy, budeme stále schopní se bavit s kamarády, kteří mají poruchu?

`bb({ eyes:"sad", body:"chest" })`

b: Pokud najdeme smír v duši, nebude nás to brzdit od dělání velkých věcí?

`hong({ MOUTH_LOCK:true })`

h: ...

h: Pokud se bojíme... "že se nebudeme ničeho bát"...

h: Mám pocit, že nám strachy jen tak nedojdou.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Uff! Ahh! Jaké to úleva!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Dotore, mám úzkosti, že platím 1000 Kč/hod, jen abych slyšela, jak se zeptáte *jak se z toho cítite?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Mm-hmm. A jak se z toho cítíš?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Meh, to zní jako naprosto pochopitelná obava.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: A stojí za prd, že mentální zdaví není dostupné pro hromadu lidí.

`hong({ eyes:"normal", mouth:"normal" });`

h: Přes to, jsou tu levnější alternativy:

`hong({ body:"chin" })`

h: Podporné skupiny, online terapie, studentská/nezisková zdravotní centra...

`hong({ body:"hands_1" })`

h: Učit se návyky jako meditace, bavit se pravidelně s kamarády, učit se nové věci, zaměřit se na kvalitní spánek...

`hong({ body:"hands_2" })`

h: Jít do knivny si půjčit knížky pro psychoterapie založené na poznatcích...

`hong({ body:"one_up" })`

h: Tady je celý seznam na konci této hry!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: No, *ta* čtvrá stěna nevydržela moc dlouho.

`hong({ body:"point" });`

h: Jsou duležitější věci než správné vypravění příběhu. Třeba mentální zdraví.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Já myslím, že to říkají terapeuti? Příjmy své emoce, i ty negativní?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Wait.

["Příjmi" jako *vzdej to*?](#act4_bad_accept_give_up)

["Příjmi" jako *schvaluj*?](#act4_bad_accept_approve)

["Příjmi" jako *ber doslova*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Myslíš si, že Martin Luther King by řekl, "Hoši, nemžeme sedět vepředu v autobuse, pojďme to *akceptovat*?"

`bb({ eyes:"angry_r", body:"two_up" });`

b: Přoč si self-help průmysl myslí, že mávat bílým praporem je nějaké *hluboké moudro?*

`bb({ eyes:"annoyed", body:"normal" });`

h: Myslím si, že terapeuti myslí "příjmi" špatné věci jako: přiznej, že existují a jsou těžké změnit,

h: Ale ne nutně se vzdát snahy to změnit.

`bb({ eyes:"suspect" });`

b: Tak by měli terapeuti říkat *přiznej*, ne *příjmi*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Jako, jak nda tím přemýšlím, "příjmi" je docela matoucí.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Tak to *přiznávám*.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Jako, kdyby bylo *dobře*, že jsme rozbití nebo tak nějak? Ne!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Všichni tihle Hollywoodští scénáristé, kteří romantizovali mentální nemoce kecají nesmysly!

`bb({ eyes:"angry", body:"two_up" });`

b: Mít mentální poruchu stojí za *prd!* Lidem to kazí *životy!* Proč bychom to měli "přijímout"?!

`bb({ body:"normal" });`

h: Myslím si, že terapeuti myslí "příjmout" naše emoce ve smyslu: měj s nimi trpělivost.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Jako soupeření s tekutým pískem tě jen potopí rychleji a řešení problému je trpělivě počkat,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Bojovat proti tobě, můj strachu, mě vedlo k tomu, abych skočila ze střechy.
{{/if}}

{{if !_.INJURED}}
h: Bojovat proti tobě, můj strachu, mě skoro vedlo k tomu, abych skočila ze střechy.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Místo toho, řešení ješení je to, co děláme teď. Nebojujeme, ale ukazujeme tomu druhému trpělivost.

`bb({ eyes:"annoyed" });`

b: Tak by měli říkat *tohle* místo nějakých problematických slov jako "příjmout".

`hong({ body:"chin", eyes:"annoyed" });`

h: Jak nad tím přemýšlím, "příjmout" stojí za prd.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: Já nepříjímám "příjmout".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Ale už *víme*, že bys mě neměla brát doslova!

`bb({ eyes:"sad_u", body:"two_up" });`

b: Celý ten *problém* je to, že já ti chci pomoc, ale stojím za prd ve vybírání těch pravých slov!

`bb({ eyes:"sad", body:"normal" });`

h: Já si myslím, že terapeuti myslí "příjímaní" svých emoci jako: "nebojuj s nimi nebo je neignoruj."

`hong({ eyes:"surprise", body:"one_up" });`

h: Vyslechnout tě, pracovat *s* tebou, ale nebrat tě jaki 100% doslovnou pravdu.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Tak by terapeuti měli říkat *tohe* míst vágního a matoucího slova jako je "příjmout".

`hong({ body:"chin", eyes:"annoyed" });`

h: Asi jim taky nejde vybírání těch pravých slov.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Každopádně, ještě něco, o čem by ses rád pobavil?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: Ještě něco tíží tvé srdce?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Bojím se, že nám bude ublíženo.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Bojím se, že skončíme osamocení.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Bojím se, že jsme špatní lidé.](#act4_bad)
{{/if}}

[Ne, to stačí.](#act4c_prelude)

# act4_something_else_2

h: Ok, myslím si, že jsme zatím probrali všechny naše strachy.

b: Ano, jsou tady jen tři strachy.

h: Jo, přesně tři.

b: Příhodné.

(#act4c)

# act4c_prelude

h: Dobrý pokec, týme.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: Tohle není nějaká *hra*, víš.

`bb({eyes:"angry_d", body:"one_up"})`

b: Vybudovat si zdravý vztah se svými emocemi není tak jednoduché, jako klikat na čudlíky na obrazovce.

`bb({eyes:"sad", body:"normal"})`

b: Vážně *můžeme* spolu vyhcázet?

b: *Můžeme* spolupracovat jako tým?

`hong({eyes:"sad", body:"one_up"})`

h: No,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: Odpusť mi...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: Měla bys problém kdybych si k tobě přisedla na oběd?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: Do *téhle* jsi se zakoukala? Proč sedí osamoťe jako nějký psychopatický sériový vrah?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Ptát se holky do které ses zakoukala, jestli si k ní můžeš sednou? Víš jak *vtěrně* zníme?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: Do *téhle* jsi se zakoukala? Narušujeme její klid a mír! Jsme takoví otravové!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: Já- Já myslím- je, je v pořádku pokud ne, já jen...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Počkej neviděla jsem tě na té párty?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Jo, samozřejmě! Pojď sem.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Promiň, ale teď potřebuji býs sama.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Jó ty jsi byla na té pohovce! Na té první párty, kam jsem šla...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Kde jsem měla záchvat paniky a jednu jsem vlepila hostiteli.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Kde jsem měla záchvat paniky a utekla jsem s brekem.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Počkej člověče, vybá to, že je jsme je vyvedli z rovnováhy.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Oh, promiň nechtěla jsem tě postavit vás do nepříjemné situace!

`publish("act4", ["hong_to_alshire",4]);`

h2: Jen si pamatuji přátelkou tvář, to je věe.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AAAAAAA JÁ TO VĚDĚLA! JE NEBEZPEČNÍ PANIKOU ŘÍZENÝ PSYCHOUŠ!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAAAAA PRVNÍ DOJEM, KTERÝ JSME UDĚLALY, JE "VIDĚLI JSME JEJÍ TRAUMA"! TO ZNAMENÁ, ŽE NÁS NENÁVIDÍ!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAAAA PŘIPOMĚLI JSME NĚKOMU JEHO NEPŘÍJEMNOU VZPOMÍNKU. NAŠE PŘÍTOMNOST UBLIŽUJE OSTATNÍM.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Zadrž človče, vypadá znás docela nesvá.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Oh, nestresuj se!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Jen říkám, že si sem můžeš sednou jestli chceš.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: JSE AŽ *MOC* PŘÁTĚLSKÁ! JAKO TEN BUNDY, SÉRIOVÝ VRAH!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: JEN PŘEDSTÍRÁ, ŽE JE MILÁ! NIKDO *VÁŽNĚ* NECHCE BÝT BLÍZKO NÁS!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAA MY VŽDY ZAVINÍME, ŽE SE OSTATNÍ CÍTÍ DIVNĚ! JSME JEN ODUTIVÉ BYTOSTI NA ZEMI!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Zadrž človče, vypadá znás docela nesvá.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Oh, já nechtěla být neurvalá!

`publish("act4", ["hong_to_alshire", 6]);`

h2: Já se jen snažím pochopit moje emoce. Prosím neber si to osobně.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: CO ZA DIVNÉ, ZVRÁCENÉ MYŠLENKY SE JIM HONÍ V HLAVE?! CO ZA TEMNÉ TOUHY NAPLŇUJÍ SRDCE TOHLE PSYCHOUŠE?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: BYLY JSME ODMÍTNUTI! NIKDY NÁS NIKDO NEBUDE MILOVAT!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: NAUŠILI JSME JIM CHÁPANÍ JEJÍCH EMOCÍ! NYNÍ BUDE NAVŽDY TRAUMATIZOVANÁ A JE TO VŠECHNO NAŠE CHYBA!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: BĚŽ BĚŽ BĚŽ BĚŽ BĚŽ BĚŽ BĚŽ BĚŽ BĚŽ BĚŽ BĚŽ BĚŽ BĚŽ BĚŽ BĚŽ

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: Huh. To bylo divné. Zajimá mě, co jí vrtalo hlavou.

`publish("act4", ["hong_closer", 2]);`

h: Každopádně, co jsi to říkal?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Ach, já zapoměl? Něco ohledně týmu a práce?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Měla bys "uzavřít mír" se svými emocemi, jako kdyby to byli nějací *váleční zločinci*.

`publish("act4", ["bb_closer", 7]);`

b: Chci aby mezi námi bylo *víc* něž jen mír! Chci aby jsme byli *spojenci!*

`publish("act4", ["bb_closer", 3]);`

b: Já chci být hodný hlídací pes. Jako hlad a žízeň jsou signaly fizických potřeb,

`publish("act4", ["bb_closer", 8]);`

b: Já chci být signál tvých *psychických* potřeb, tých potřeb na bezpečí, soundaležitost a dobrosrdečnost.

`publish("act4", ["bb_closer", 1]);`

b: Ale... moje práce stojí za prd, takže budu potřebovat od tebe trochu vycvičit.

`publish("act4", ["bb_closer", 4]);`

b: Ne vždy "mám pravdu," ani nejsem "vždy iracionální." Já se jen... snažím dělat to nejlepší. Tak, prosím,

`publish("act4", ["bb_closer", 30]);`

b: Pomoc mi ti pomáhat!

`publish("act4", ["bb_closer", 6]);`

b: Ačkoliv, učit starého psa novým triků chvilku *zabere*. Možná *roky.*

`publish("act4", ["bb_closer", 3]);`

b: A někdy se mi to možná vrátí, a já zase spadnu do starých kolejí.

`publish("act4", ["bb_closer", 2]);`

b: Budu štěkat na stíny. Strašit tě slovy. Možná ti budu ukázovat nějaké vtíravé obrázky... věcí.

`publish("act4", ["bb_closer", 9]);`

b: Já se omlouvám! Jsem pošramocený pes z útulku! Pošramocení psi se ti občas vykadí do postele!

`publish("act4", ["bb_closer", 4]);`

b: Ale jestli budeš se mnou trpělivá... a zůstaneš a sedneš si se mnou...

`publish("act4", ["bb_closer", 8]);`

b: Možná skrotíš toho vlka.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Hodný pejsek.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Hodný člověk.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: AAAAA STÁLE JÍŠ SAMA PATNÁCT CIGARET AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA STÁLE NEJSI PRODUKTIVNÍ KDYŽ JÍŠ JSME SOCIÁLNÍ PARAZITI AAAAA
{{/if}}

{{if _.whitebread}}
b: AAAAA JÍŠ VÍCE BÍLÉHO PEČIVA AAAAA
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: YAP YAP YAP YAP YAP

(#credits)
