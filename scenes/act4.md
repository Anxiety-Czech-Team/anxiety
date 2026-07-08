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

h: *sigh*

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

b: And yet...

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

b: Nejsem Velký zlý vlk. Ale nejsem ani strážný vlk.

`bb({eyes:"sad_d"})`

b: Jsem týraný pes z útulku.

`bb({eyes:"sad"})`

b: Prošli jsme si těžkými věcmi. Možná trauma nebo zanedbávání. Proto někdy reaguji přehnaně a odcházím:

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
b: Nevím, už dost toho, že si vybírám, co řeknu dál. Co říkáš *ty*, člověče?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Znovu se vracím k tobě, člověče. Co si myslíš?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Další myšlenky, člověče?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Máte pravdu. Tak se chraňme.](#act4_harm_skills)

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

h: Právě teď si procvičujeme dobrou komunikaci. Což nám pomůže lépe odhalit nebezpečí, s menším počtem falešných poplachů,

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

h: Ale i 1% zlepšení má svou cenu, že?

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

[Jsem vla a ne pes.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

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

h: Pracovaním a vyjednávaním s tebou tu hranici někde vytyčíme.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Dobře. Ale já nemám protilehlé palce, takža to zapíchávání kolíků je na tobě.

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

h: To je přesně proč, kdybycho začali expoziční terapii, tak začneme pomalu a malými krůčky kupředu.

h: Právě před tím než narazíme na *skutečné* nebezpečí, zastavíme.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Já vymezuji hranici mezi tím, že slyším vzdáleného hromu a stáním v bouřce se špičatou čepicí.

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

h: Jo! Děkuji ti, že jsi se staral o moje {{_.thanks_for}}.

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

b: Počkej... neříkáš furt dokola "děkuji ti", aby ses vyhnula mluvit o tvých straších, že ne?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Víš, je to komplikované a já nebudu mít vždy připravené odpovědi.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Život ti ale nedává seznam tři předpřipravených dialogových odpovědí.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Ale prozatím, mohu alespoň poděkovat.

b: No, já děkuji tobě taky, za trpělivé vysvětlování.

`bb({ eyes:"closed" });`

b: Ty malé bezchlupý savče z masa a kostí.

(#act4_something_else)

# act4_thanks_3

h: I když mě tvé žvaňění straší, snažíš se prostě chránit moje {{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: Dobře, jestli mi budeš skládat komplimenty, tak internet si o nás bude myslet divné věci.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Ale, já jsem jen zranitelná holka a ty jsi velký, zlý vlk. Co nejhoršího se můž--

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

b: Já se ale bojím, že pokud někdo nás pozná, naše skutečné já, tak je vyděsíme a utečou.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Já ti nevím, dost *mě* vybírající, co řeknu dál. Co na to říkáš *ty*, člověče?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Zase, zpět k tobě, člověče. Co si myslíš?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Nějake další návrhy, člověče?
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

h: Mohli bychom se naučit nějaké schopnosti jako: ptát se na otázky, naslouchání, empatie, otevírat se novým myšlenkám a být zranitelný, atd?

`hong({ eyes:"normal_l" });`

h: Či si udělat lepší sociální návyky, jako plánovaní volného času s kamarády nebo pravidelně chodit na srazy?

`hong({ body:"one_up" });`

h: Také se naučit být víc v pohodě s odmítnutím.
`hong({ eyes:"normal" });`

h: Nebo se naučit poznat kdy lidi *nejsou* na nás naštvaní, jsou jen unaveni z našeho ksichtění.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: To je hromada možností. Ale, ohledně "učení se sociálních schopností"...

[Není to *manipulativní?*](#act4_alone_skills_manipulative)

[Neučiní nás to *náchylnější na manipulace?*](#act4_alone_skills_manipulated)

[Co, když i přes to selžeme?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Nejsou sérioví kteří čtou emoce jejich obětí dobří v empatii?

`bb({ eyes:"annoyed" });`

b: Nezískával si Charles Manson přátele a neměl vliv na lidi?

`hong({ eyes:"annoyed", body:"chin" });`

h: Ano, máš pravdu.

h: "Sociální schopnosti" neznamenají nic, pokud nás pokud *o* lidi nemáme upřímný zájem.

`hong({ body:"normal" });`

h: Prostě, nebuď ^kokot^.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: To bych chtěl jako motivační popisek na plakát.

`hong({ body:"shrug", mouth:"narrow" });`

h: “Prostě, Nebuď ^Kokot^™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Budeme jako vítací rohožka, říkat Prosím a Děkuji Ti jako by si lidi o nás otírali boty!

`bb({ mouth:"scream", eyes:"scream" })`

b: Políbíme tolik zadků, že to bude vypadat, že nosíme hnědou rtěnku!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Jo, máš pravdu. "Sociální dovendosti" nemohou být jen o tom uspokojovat ostatní, taky by to mělo být o nastavování *hranic*.

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

h: To je v pořádku! Selhání je jak se všichni učíme novým věcem!

`hong({ body:"normal", eyes:"normal" });`

h: Tak pojďmě společně selháním kupředu, jo?

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

h: Můžeme pošťouchnout kamaráda, aby jsme se potkali, setkání po letech se starým brachem, nebo jen pokecat s baristou.

`hong({ body:"normal" });`

h: Myslím si, že můžeme zjistit, že jsme oblíbenější, než si myslíme.

`bb({ eyes:"annoyed" });`

[Co když tohle jsou jen malá, levná "vítezství"?](#act4_alone_experiment_cheap)

[Co když tohle je zátěž pro ostatní?](#act4_alone_experiment_burden)

[Ale *small talk* není to *pravé* my!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Pokud nasadímé mělký úsměv, nikdy nebudeme schopni se propojit s kýmkoliv,

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

h: Jednoho dne budeme moci ukázat lidem naše pravá já, naprosto robité, naprosto lidské.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Já se převalím, pokud mi dáš pamlsek.

`bb({ eyes:"normal", mouth:"normal" });`

h: Ne.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Řikat "ahoj" baristovi není úplně olympijský výkon v disciplíně sociálního přizpůsobování.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Je to pro *nás!*

`hong({ body:"one_up", eyes:"annoyed" });`

h: V ringu sociálních schopností jsme nesme ani v peříčkové váhové kategorii. Jsme spíše... kvarková váhová kategorie.

`hong({ body:"normal", eyes:"normal" });`

h: A někde musíme začít a jestli to mají být jednoduchá vítězství, tak ať. Musíš udělat ten první krok než uděláš tes tisícátý.

b: Jo! Možná po tom co řekneme "Ahoj", můžeme pokračovat a říct...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Jak se máš?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Nic moc!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Maybe the barista just wants to make some dang coffee, not be an *experiment* to see if our social skills suck.

`bb({ eyes:"annoyed" })`

h: Well, if it turns out we *are* being a burden...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: That's good to know, too!

`hong({ eyes:"normal" });`

h: We can then learn how to pro-actively ask people what they're comfortable with, to know and respect others' boundaries.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Y'know, all that "inter-personal skills" ^crap^ we see in counselor brochures.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: I want to defend your moral needs, that drive to become a better person,

`bb({ eyes:"sad_d" })`

b: But it just feels like deep down, we're so fundamentally... broken.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: And don't tell me we're *not* messed up. We jumped off a *roof*.
{{/if}}

{{if !_.INJURED}}
b: And don't tell me we're *not* messed up. We almost jumped off a *roof*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: I dunno, enough of *me* choosing what to say next. What do *you* say, human?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Again, back to you, human. What do you think?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: More thoughts, human?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[So we're broken. Let's fix us.](#act4_bad_fix)

[So we're broken. Let's accept it.](#act4_bad_accept)

[Thank you.](#act4_thanks) `_.thanks_for = "moral well-being";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: We could slowly build better habits, get our life more in line with what we value,

`hong({body:"one_up"});`

h: And if needed, we could get professional help – a therapist or counsellor.

`hong({body:"normal"});`

h: There's ways to fix us.

[What if we can't fix it all?](#act4_bad_fix_cant)

[What if we fix *too* much?](#act4_bad_fix_too_much)

[We can't afford professional help.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Nah, I guess you're right.

h: We can't fix it all.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ahhh I knew it we'll always be broken!

`hong({eyes:"surprise"});`

h: But we can at least be *less* broken.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Scars heal with time, but they never go away. And that's okay.

`bb({eyes:"annoyed_r"});`

b: I guess. Besides,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Scars are *sexy.*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Please do not do that.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: This feels sick to admit, but... some part of me *wants* to have this disorder.

`bb({ eyes:"angry" })`

b: I mean, without it, won't we be *boring?*

`bb({ eyes:"sad_r", body:"one_up" })`

b: Without the disorder, won't our art become stale and bland?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Without the disorder, won't we be unable to connect with our friends who have the disorder?

`bb({ eyes:"sad", body:"chest" })`

b: If we're ever content with life, won't we stop driving ourselves to do great things?

`hong({ MOUTH_LOCK:true })`

h: ...

h: If we even fear... "running out of fears"...

h: I don't think we're gonna run out of fears.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Oh, yeah! Whew! What a relief!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Doc, I'm anxious that I'm paying $100/hr just to hear you ask *how does that make you feel?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Mm-hmm. And how does that make you feel?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Nah, that's a totally reasonable worry.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: And it genuinely sucks that mental healthcare isn't affordable for lots of folks.

`hong({ eyes:"normal", mouth:"normal" });`

h: Still, there are some cheap or free options:

`hong({ body:"chin" })`

h: Support groups, online therapy, student/non-profit health centers...

`hong({ body:"hands_1" })`

h: Building habits like meditation, sleeping well, chatting regularly with friends, learning new things...

`hong({ body:"hands_2" })`

h: Going to a library to borrow workbooks for evidence-based psychotherapies...

`hong({ body:"one_up" })`

h: There's a full list of resources at the end of this game!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Well *that* fourth wall didn't last long.

`hong({ body:"point" });`

h: Some things are more important than narrative convention. Such as mental health.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: I mean, that's what therapists say right? Accept all your emotions, even the negative ones?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Wait.

["Accept" as in *give up*?](#act4_bad_accept_give_up)

["Accept" as in *approve*?](#act4_bad_accept_approve)

["Accept" as in *take literally*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Do you think Martin Luther King would've said, "Shucks we can't sit in the front of the bus, let's just *accept* it?"

`bb({ eyes:"angry_r", body:"two_up" });`

b: Why does the Self-Help Industrial Complex think waving the white flag is some *profound wisdom?*

`bb({ eyes:"annoyed", body:"normal" });`

h: I think therapists mean "accept" bad things as in: acknowledging they exist and are hard to change,

h: But not necessarily giving up a commitment to change.

`bb({ eyes:"suspect" });`

b: Then therapists should say *acknowledge*, not *accept*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Yeah come to think of it, "accept" is kinda confusing.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Well, I *acknowledge* that.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Like it's *good* that we're broken or something? No!

`bb({ eyes:"angry_r", body:"one_up" });`

b: All those dang Hollywood screenwriters who romanticize mental illness are full of crud!

`bb({ eyes:"angry", body:"two_up" });`

b: Having a mental disorder *sucks!* It robs people of *lives!* Why should we "accept" that?!

`bb({ body:"normal" });`

h: I think therapists mean "accept" our emotions as in: be patient with them.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Like how struggling in quicksand makes you sink faster, and the solution is to patiently lie flat,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Fighting against you, my fear, led me to jump off a roof.
{{/if}}

{{if !_.INJURED}}
h: Fighting against you, my fear, almost led me to jump off a roof.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Instead, the solution is to do what we're doing now – not to fight, but to patiently be with each other.

`bb({ eyes:"annoyed" });`

b: Then they should say *that* instead of some problematic word like "accept".

`hong({ body:"chin", eyes:"annoyed" });`

h: Yeah come to think of it, "accept" kind of sucks.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: I do not accept "accept".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: But we already *know* you shouldn't take me literally!

`bb({ eyes:"sad_u", body:"two_up" });`

b: The whole *problem* is that I want to help you, but I suck at using words to do so!

`bb({ eyes:"sad", body:"normal" });`

h: I think therapists mean "accept" your emotions as in: "don't fight or ignore them."

`hong({ eyes:"surprise", body:"one_up" });`

h: To listen to you, work *with* you, but not take what you say as 100% literal truth.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Then therapists should say *that* instead of some vague confusing word like "accept".

`hong({ body:"chin", eyes:"annoyed" });`

h: I guess they suck at using words, too.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Anyway, anything else you wanna chat about?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: So, anything else on your heavy heart?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[I'm scared we'll be harmed.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[I'm scared we'll be alone.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[I'm scared we're bad people.](#act4_bad)
{{/if}}

[Nah, I'm good for now.](#act4c_prelude)

# act4_something_else_2

h: Okay, I think we've talked about all our fears now.

b: Yes, there are only three fears.

h: Yup, exactly three.

b: Convenient.

(#act4c)

# act4c_prelude

h: Good chat, team.

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

b: This isn't some *game*, you know.

`bb({eyes:"angry_d", body:"one_up"})`

b: Building a healthy relationship with your emotions isn't as simple as clicking buttons on a screen.

`bb({eyes:"sad", body:"normal"})`

b: *Can* we really get along?

b: *Can* we work together, as a team?

`hong({eyes:"sad", body:"one_up"})`

h: Well,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: E-excuse me...

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

a: W-wo-would you mind if I sat with you for lunch?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *This* is your crush? Why are they sitting alone like a psycho serial killer?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Asking your crush if you can sit with them? Do you know how *needy* we sound?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *This* is your crush? We interrupted their peace and quiet! We're such a burden!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: I- I mean- it's, it's okay if not, I just...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Wait, didn't I see you at the party?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Yeah, of course! Come here.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Sorry, I need alone time right now.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Yeah you were on the couch! At the first party I went to...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Where I had that panic attack and punched the host.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Where I had that panic attack and ran out crying.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Hang on human, we may be making them uncomfortable.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, I don't mean to put you on the spot!

`publish("act4", ["hong_to_alshire",4]);`

h2: Just remembering a friendly face, is all.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHHHH I KNEW IT! THEY'RE A DANGEROUS PANIC-DRIVEN PSYCHO!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHHH THE FIRST IMPRESSION WE MADE WAS "WITNESSED MY TRAUMA"! THAT MEANS THEY HATE US!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAHHH WE MADE SOMEONE REMEMBER A TRAUMATIC EVENT. OUR MERE PRESENCE HURTS OTHERS.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Hang on human, they seem uncomfortable.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, no pressure of course!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Just saying, you can sit here if you want to.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: THEY'RE BEING *TOO* FRIENDLY! LIKE TED BUNDY, THE SERIAL KILLER!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: THEY'RE JUST ACTING NICE! NO ONE *REALLY* WANTS TO BE CLOSE TO US!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH WE ALWAYS MAKE OTHERS FEEL AWKWARD! WE'RE A STAIN UPON THE EARTH!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Hang on human, we may be making them uncomfortable.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, I don't mean to be rude!

`publish("act4", ["hong_to_alshire", 6]);`

h2: I just need some time to process my emotions. Please don't take it as a personal rejection.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: WHAT SICK, TWISTED THOUGHTS ARE THEY PROCESSING?! WHAT DARK DESIRES FILL THIS PSYCHO'S HEART?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: WE'VE BEEN PERSONALLY REJECTED! WE'LL NEVER BE LOVED!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: WE INTERRUPTED THEIR EMOTIONAL PROCESSING! NOW THEY'LL BE TRAUMATIZED FOREVER AND IT'S ALL OUR FAULT!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN

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

h: Huh. That was weird. I wonder what was going on in their head.

`publish("act4", ["hong_closer", 2]);`

h: Anyway, you were saying?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Uh, I forget? Something about teams and work?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: They say you should "make peace" with your emotions, as if your emotions are *war criminals*.

`publish("act4", ["bb_closer", 7]);`

b: But I want us to make *more* than mere peace! I want us to be *allies!*

`publish("act4", ["bb_closer", 3]);`

b: I want to be a good guard-dog. Just like how hunger & thirst are alarms for your physical needs,

`publish("act4", ["bb_closer", 8]);`

b: I want to be the alarm for your *psychological* needs – your needs for safety, belonging, goodness.

`publish("act4", ["bb_closer", 1]);`

b: But... I suck at my job, so I need you to train me.

`publish("act4", ["bb_closer", 4]);`

b: I'm not "always valid," nor "always irrational." I'm just... trying my best. So, please,

`publish("act4", ["bb_closer", 30]);`

b: Help me help you!

`publish("act4", ["bb_closer", 6]);`

b: Though, teaching an old dog new tricks *will* take a while. Maybe *years.*

`publish("act4", ["bb_closer", 3]);`

b: And sometimes I'll relapse, I'll slip into my old habits.

`publish("act4", ["bb_closer", 2]);`

b: I'll bark at shadows. I'll scare you with words. I might even show you some intrusive images of... things.

`publish("act4", ["bb_closer", 9]);`

b: I'm sorry! I'm a battered shelter dog! Battered dogs poop on your bed sometimes!

`publish("act4", ["bb_closer", 4]);`

b: But if you're patient with me... and just stay and sit with me...

`publish("act4", ["bb_closer", 8]);`

b: Maybe you can tame this wolf.

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
