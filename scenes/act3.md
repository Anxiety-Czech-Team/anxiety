# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Nazdraví!

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *Joo* to mi bodlo.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: Víš, špunte...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: Přesněji, přesněji mi to bodlo do pravé a levé amygdaly.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Připomínáš mi, když jsem byl mladší. Tehdy, když mě trýznilo to zvíře v hlavě.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: Jsem tak rád, že ti to mohu oplatit a pomoct ti zabít to zvíře stejně, jako jsem já zabil to svoje.

```
publish("act3",["roofhunter",2]);
```

r: Hej, rychlá otázka: pravda, nebo výz--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: VÝZVA!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Haha! Dobře.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Ok. Vidíš tam dole ten světle modrý bazén?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Jo? Šest pater dole?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Skoč do něj.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Počkat, co?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: Zvířátko začalo skučet?

```
publish("act3",["roofhunter",23]);
```

r: *Ale neee je to nebezpečné, neděleeej toooo.*

```
publish("act3",["roofhunter",22]);
```

r: Ale to je přesně proč potřebuje zážitky blízké smrti! Pořádně si zapař! Carpe diem! Šnupni si kokain ze zadku ^štětky^, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: Ukaž tomu zvířeti, že nedáváš *^mrd^* ohledně jeho tlachání! Skákej.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Ahh, ale občas, ahh... strach má nějaký důvod...

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: Já se obávám, že jsi padla za oběť propagandě panstva dokonalých, co se ti snaží nabulíkovat, že cítit se špatně je *dobré*?

```
publish("act3",["roofhunter",17]);
```

r: Ti ^sráči^, co ovládají svět, dávají *nám*, zbytku, úzkosti a deprese,

```
publish("act3",["roofhunter",18]);
```

r: Pak nám dají přednášku, abychom "přijali" to, že nás ^ojebou^, a "uvítali" toho sadistického demona v naší hlavě!

```
publish("act3",["roofhunter",6]);
```

r: Špunte, já vím, že *ty* víš, že to zvíře *ubližuje* lidem, jako jsme my. *Trýzní* to lidi, jako jsme my.

```
publish("act3",["roofhunter",19]);
```

r: Není to náš přítel. Je to vzteklé zvíře, které musí být *uspáno*,

```
publish("act3",["roofhunter",20]);
```

r: Nebo vložit *trochu olova do jeho lebky*.

```
publish("act3",["roofhunter",27]);
```

r: Jinak ho necháš vyhrát.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: Ne. Nemáš pravdu.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: Nenechám ho vyhrát.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: Do ^prdele^! Já ti věřím, kotě! Zab ho! <3

(#act3a)



# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: ne ne ne ne ne ne

n: TATO KAPITOLA MÁ 2 MOŽNÉ KONCE. JEDEN JE *VELMI, VELMI ŠPATNÝ.*

b: NE NE NE NE NE NE NE NE NE NE NE NE NE NE

n: VYBÍREJ MOUDŘE. CHRAŇ SVÉHO ČLOVĚKA

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAA

`bb({ mouth:"normal" });`

n: HODNĚ ŠTĚSTÍ

```
Game.clearText();
bb({ eyes:"start" });
```

[Člověče, tady můžeš reálně umřít!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[Tohle je hloupé a sebedestruktivní!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Tihle magoři nejsou tví praví kamarádi!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Č--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: T--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: T--

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Víš, možná bych ti věřila... kdybys to nezkusil zilionkrát předtím.

h: Ty jsi vlk, který volal o pomoc.

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`


# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: To jsi taky zkoušel.

b: člověče, prosím...

`hong({ eyes:"look_right" });`

h: Ach promiň, že farmaceutický průmysl neschvaluje mou medikaci.

h: Podívej ^hajzle^, *všichni* máme nějaký způsob, jak tě donutit sklapnout.

`hong({ body:"look_up", eyes:"look_up" });`

h: Někteří se vrhají horlivě na práci.

`hong({ body:"look_down", eyes:"look_down" });`

h: Někteří se vrhají do světa sexu, drog a sledování feedu na Facebooku.

`hong({ body:"normal", eyes:"look_right" });`

h: Někteří se vrhají do náruče jiných lidí. 

`hong({ eyes:"angry" });`

h: Já se vrhnu do toho bazénu.

[Jsi opilá a je to ŠEST PATER](#act3_bad_1_harm)

[Sakra, tohle je to poděkování, které dostanu?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Dobře, přiznávám. Pokazil jsem to.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: I kdybys dopadla do vody, tak povrchové napětí ti zlomí žebra a budeme mít otřes mozku *minimálně*

h: Uhh.

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Jednou jsem viděla na YouTube Rusáky, jak to dělají.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: Já- Promiň, jaké *poděkování?*

`bb({ eyes:"angry" });`

b: Tohle je přesně, proč *existuji!* Protože lidem se nedá věřit, že se zvládnou ochránit sami!

b: Já jsem se snažil ochránit tvou hloupou maličkost celý svůj život a nyní ty prostě bud--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: huh.

`hong({ body:"laugh_2" })``

h: hahahaha

`hong({ body:"laugh_3" })``

h: HAHAHAHAHAHA

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: Ah. WOW je to ^kurva^ největší podhodnocení celého století!

`hong({ body:"yell_2" });`

h: Jo, ty hnijící kupo zakrvácených ^hoven^! Tohles ^kurva^ posral!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Nějaké další námitky, pane Samozřejmý?

[Ale pomsta není odpověď!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Ale tentokrát mám *reálně* pravdu!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Ublížil jsem ti.](#act3_good_2a)


# act3_good_1_fail_revenge

b: Potřebuješ mít zdravější vztah se svými emocemi a ne je utápět v alk--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)



# act3_good_1_fail_harm

b: Tak prosím, polož tu láhev a pojďme--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)




# act3_bad_2

`bb({ eyes:"sad" });`

b: prosím... nedělej to...

h: Tvůj ukazatel energie vypadá podezřele nízce, vlku.

h: Být tebou, tak volím svá slova velmi opatrně.

`bb({ eyes:"normal" });`

[Budiž. Já už končím s tím, že tě chráním.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Měl jsem celou dobu pravdu.](#act3_bad_2_right)

[Já se omlouvám.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: No tak, do toho, skoč. Co mi je po tom.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Tak jo. Do dna.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: POČKEJ, NE, TO BYLA OBRÁCENÁ PSYCHOLOGIE TY JSI MĚLA UDĚLAT *OPAK* NEŽ CO JSEM ŘE--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: Ty se sama stavíš do nebezpečí. Ti tvoji takzvaní kamarádi tě využívají a ty využíváš tvé takzvané kamarády.

`bb({ eyes:"sad" });`

b: Tak prosím, člověče... proč mi nevěříš?!

h: Protože ty jsi nikdy nevěřil ve *mě*.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Ostatní hlídací psi mají lidi, kteří je trpělivě vycvičili, aby se *naučili* spolupracovat,

b: Místo toho, aby nenáviděli hlídací psy snažící se je chránit! Tak proč nemůžeš pros--

`bb({ eyes:"normal" });`

h: Špatná, ^debil^ní odpověď.

(#act3_bad_3)



# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *"Jediná věc, které se máme bát, je strach sám."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Don't worry, be happy!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Všichni moudří lidé naší doby souhlasí: negativní emoce jsou *špatné!*

`hong({ eyes:"less_angry" });`

h: Hej! Proto se jim říká *negativní!*

b: člověče... prosím...

`hong({ eyes:"normal" });`

h: Chvíli zpátky jsem řekla: “Já už nechci nikdy cítit tuhle bolest.”

h: A mé přání se vyplnilo. Já už necítím ani bolest, ani strach, ani úzkosti...

h: Já vůbec nic necítím.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Byl jsem tak posedlý tím, aby ti nic neublížilo, že jsem si neuvědomil, že ti ubližuji já.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: NE. H^OVNO^.

`hong({ body:"yell_1" });`

h: DO ^PRDELE^. To ti fakt trvalo tak dlouho na to přijít?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Mohl jsi nám ušetřit tolik problémů, ty velký chlupadý blečku. Proč jsi si to neuvědomil dříve?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...ty se *omlouváš.*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: Promiň za *co*?

(#act3_good_2q)


# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized)
{{/if}}


# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[Promiň, že jsem nebyl dobrý ochránce.](#act3_good_3_protector)

[Promiň, že jsem tě nerespektoval.](#act3_good_3_respect)

[Já se omlouvám.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Já se omlouvám, že mám hruzného člověka!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Já se omlouvám, že jsem tě nerespektvoal.](#act3_good_3_respect)

[Já se omlouvám, že jsem ti ublížil.](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: Je mou poviností tě varovat před *realnými* hrozbami, ale já jsem furt štěkal po autech a pošťákovi.

`bb({eyes:"sorry_up"});`

b: Štěkal na stíny. Štěkal tak moc,

`bb({eyes:"sorry"});`

b: že dává smysl, že jsi mi chtěla nandat náhubek.

`bb({eyes:"sorry_down"});`

b: Já se omlouvám.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: Měl jsem být *tvůj* věrný hlídací pes, ale choval jsem se, jako bys ty měla poslouchat *mě*.

`bb({eyes:"sorry_up"});`

b: Je tu rozdíl mezi ochráncem a vězeňským bachařem. Já tuto linii překročil.

`bb({eyes:"sorry_down"});`

b: Já se omlouvám.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Byl jsem tak posedlý tím tě chránit, aby sis neublížila, že jsem nikdy nezastavil a nezamyslel se, abych si uvědomil, že já ti ubližuju.

`bb({eyes:"sorry_up"});`

b: Byl jsem špatný pes.

`bb({eyes:"sorry_down"});`

b: Já se omlouvám.

(#act3_good_4)


# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: Jo, víš, tohle byl celkově blbý nápad.

h: Já jsem tohle udělala jen, aby tě to naštvalo a, vidíš, naštvala jsem tě.

h: Co tohle kolo prohlásit za remízu, dobré?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Dobré.

h: Dobré.

n: *REMÍZA*

`_.a3_ending = "walkaway";`

(#act3_end)









# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}






# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: Ah, *neblbni*. Po všem co ti to zvíře udělalo. Ty to prostě *vzdáváš*?

r: Copak se děje, špunte? *Bojíš se?*

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Ano.

h2: Bojím se.

`publish('hong-next')`

h2: A je to v pořádku!

`publish('hong-next')`

h2: Je v pořádku se bát.

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: Zamkla právě ty dveře?

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)




# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```
(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: ne...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: ne ne ne

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: NE!

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
