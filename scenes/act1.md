# act1

```
SceneSetup.act1();
```

(...300)

n: A TOTO JE ÚZKOST ČLOVĚKA

n: _TY_ JSI TA ÚZKOST

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Oh ahoj! My jsme zase zpátky?

`hong({eyes:"0_neutral"})`

n: TVÝM ÚKOLEM JE CHRÁNIT SVÉHO ČLOVĚKA PŘED *NEBEZPEČÍM*

`bb({eyes:"look", mouth:"small_lock"})`

n: VE SKUTEČNOSTI JE PŘEHRÁVÁNÍ TÉTO HRY PRÁVĚ TEĎ VYSTAVUJE *NEBEZPEČÍ*

n: RYCHLE, VARUJ JE!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Člověče! Poslouchej, jsme v nebezpečí! Hráč ...

[...nás zase bude mučit!](#act1_replay_torture)

[...nenajde alternativní konec!](#act1_replay_alternate)

[...pocítí nesoulad mezi hratelností a příběhem hry!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Donutí nás schoulit se do klubíčka a plakat!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Donutí nás ti zabít telefon za to, že ti způsobil záchvat paniky!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Donutí nás *NE*praštit hostitele večírku!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Donutí nás praštit toho Sympatického anti-padoušského hostitele večírku!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: No, aspoň tentokrát možná neskočeme ze stře--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: DONUTÍ NÁS SKOČIT ZE STŘECHY.
{{/if}}

`bb({body:"fear"});`

b: VŠECHNY TYTO NOVÉ HROZNÉ VĚCI SE NÁM STANOU A PAK--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Jasně, příběh jako *celek* je stejný, ale každá kapitola má dva možné konce a navíc všechny možnosti větvení dial--

`bb({body:"fear"});`

b: Hráč bude zklamaný, zavře tuto kartu prohlížeče, smaže náš software a pak--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Obscénní - co?

`bb({eyes:"normal"});`

b: Příběh byl o tom, že si můžete *VYBRAT* a vybudovat zdravou spolupráci se svým strachem,

`bb({eyes:"normal_right"});`

b: Ale opakování této hry vám dá stejný příběh, což znamená, že na vašich *VOLBÁCH* nezáleží,

`bb({eyes:"narrow_eyebrow"});`

b: To ukazuje rozpor mezi herním poselstvím a herní mechanikou,

`bb({eyes:"fear"});`

b: A rozplétá strukturu tohoto narativního vesmíru,

`bb({body:"fear"});`

b: A potom--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: UMŘEMEEEEEEEEEEEEE

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: Dobře, vraťme se k postavě.

```
Game.clearText();
```

n4: (NECH _SVOU_ ÚZKOST BLAH BLAH BLAH NEJVÍC PODOBNĚ TOMU, JAKO _SVŮJ_ STRACH BLAH BLAH VÍŠ O ČEM MLUVÍM)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: No super, můj vlk je zpátky. Fantastickýýý.

`hong({eyes:"0_neutral"})`

n: TVOJE PRÁCE JE CHRÁNIT ČLOVĚKA PŘED *NEBEZPEČÍM*

`bb({eyes:"look", mouth:"small_lock"})`

n: VE SKUTEČNOSTI JE TEN SENDVIČ VYSTAVUJE *NEBEZPEČÍ* PRÁVĚ TEĎ

n: RYCHLE, VARUJ JE!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Člověče! Poslouchej, jsme v nebezpečí! To nebezpečí je...

`bb({body:"squeeze"})`

n4: (NECH _SVOU_ ÚZKOST JÍT SI HRÁT! VYBER, CO NEJVÍC ODPOVÍDÁ TOMU, CO TI ŘÍKÁ _TVŮJ_ STRACH)

(#act1_normal_choice)

# act1_normal_choice

[Znova na obědě jíme o samotě! Znova!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Nejsme produktivní, když jíme!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Ten bílí chleba je pro nás špatný!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Copak nevíš že samota je spojená s předčasnou smrtí stejně jako kouření 15 cigaret denně?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Um, díky za uvedení tvých zdrojů, ale --

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Což znamená, že pokud se *hned teď* s někým nesetkáme tak-

`bb({body:"panic"})`

b: UMŘEMEEEEEEEEEEEEEEEE

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: POUŽILI JSTE *STRACH Z OPUŠTĚNÍ*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Vytáhni svůj laptop a začni pracovat, hned teď!

`hong({eyes:"0_annoyed"})`

h: Um, Nevim jesi se mi úplně chce si drobit do kláve--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Pokud nepřispíváme do těla společnosti, tak jsme parazit společnosti!

b: tělo společnosti půjde k doktoru společnosti pro léky na parazity společnosti a my--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: UMŘEMEEEEEEEEEEEEEEEE

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: POUŽILI JSTE *STRACH Z VLASTNÍ ŠPATNOSTI*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Byly tyto studije replik--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Zpracovaná pšenice nám vystřelí cukr v krvi tak vysoko, že nám budou muset amputovat všechny končetiny a my-

`bb({body:"panic"})`

b: UMŘEMEEEEEEEEEEEEEEEE

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: POUŽILI JSTE *STRACH ZE ZRANĚNÍ*

(#act1b)

# act1b

n: JE TO SUPER EFEKTIVNÍ

`bb({mouth:"smile", eyes:"smile"});`

b: Vidíš, člověče? Já jsem tvůj věrný strážný vlk!

`bb({body:"pride_talk"});`

b: Věř své intuici! Tvé pocity jsou vždy odůvodněné!

`bb({body:"pride"});`

n: SNIŽTE ENERGETICKOU HODNOTU SVÉHO ČLOVĚKA NA NULU

n: PRO OCHRANU JEJICH FYZICKÝCH + SOCIÁLNÍCH + MORÁLNÍCH POTŘEB, MŮŽETE POUŽÍT:

n: STRACH ZE *ZRANĚNÍ* #harm#

n: STRACH Z *OPUŠTĚNÍ* #alone#

n: A STRACH Z *VLASTNÍ ŠPATNOSTI* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n: (POZNÁMKA: POUŽIJ TY VOLBY, KTERÉ TI OSOBNĚ ZASÁHNOU DO NEJHLUBŠÍCH, TEMNÝCH STRACHŮ!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: víš co, možná, že je čas se kouknout na mobil.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: OCHRAŇ SVÉHO ČLOVĚKA

n: OD SVĚTA. OD OSTATNÍCH LIDÍ. OD SEBE SAMA.

n: HODNĚ ŠTĚSTÍ

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: PRVNÍ KOLO: *BOJUJTE!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Huh. Facebook hlásí, že se tento víkend koná párty.

`bb({eyes:"uncertain"});`

b: Nepořádá ten podivín párty *každý* víkend?

`bb({eyes:"uncertain_right"});`

b: Jakou vnitřní prázdnotu se snaží zaplnit? Musí mít uvnitř uplný chaos!

`hong({eyes:"surprise"});`

h: A taky jsme dostali pozvánku?

`bb({eyes:"fear", mouth:"normal"});`

b: Tak tedy!

[Řekni ano, nebo umřeme na osamělost!](#act1c_loner)

[Řekni ne, je to tam plné jedovatých drog!](#act1c_drugs)

[Ignoruj to, jen děláme večírky smutné.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Patnáct cigaret denně, člověče! Patnáct!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: Pak se nikdo neoběví na našem pohřbu, vysypou náš popel do oceánu, budeme sežráni velrybou,
{{/if}}

{{if !_.fifteencigs}}
b: a staneme se VELRYBÍM TRUSEM!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: Takže jo, měli bychom jít na tu párty!
{{/if}}

{{if _.parasite}}
b: Jen si dones laptop, ať můžeme pracovat a nebýt parazity společnosti.
{{/if}}

{{if _.whitebread}}
b: Jen pokud nepodávají BÍLÝ CHLEBA
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: BOŽE. Pokud tě to umlčí, fajn.
h: Řeknu ano.

{{if _.whalepoop}}
b: Velrybí trus, člověče! Velrybí trus!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: nebo ještě hůř... BÍLÝ CHLEBA
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Předávkujeme se tolik pervitinem a bílým chlebem, že se naše tlustá mrtvola nevejde do kremační pece!
{{/if}}

{{if !_.whitebread}}
b: Předávkujeme se tolika drogama, že se pohřebník bude divit, jak je možný, že naše tělo bylo *už* předem nabalzamováno!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Kromě toho, nemůžeme pařit, musíme pracovat, nebo jsme hrozní společenskí paraziti!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: BOŽE. Pokud tě to umlčí, fajn.

h: Řeknu ne.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Vždycky jenom brečíme v koutě o tom, jak je samota stejně smrtící jako 15 cigaret denně.
{{/if}}

{{if _.parasite}}
b: Na večírcích se jen trápíme tím, jak bychom měli být místo toho produktivní.
{{/if}}

{{if _.whitebread}}
b: Na večírcích se jen trápíme tím, jaké tam mají nezdravé jídlo které nás zabije.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: jé, zajímalo by mě proč.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Takže když půjdeme, budou se cítit špatně, ale když odmítneme, tak se taky budou cítit špatně!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: VŠE, CO DĚLÁME, JE, ŽE V LIDECH VYVOLÁVÁME ŠPATNÉ POCITY, MĚLI BYCHOM SE TAKY CÍTIT ŠPATNĚ

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Ugh. Pokud tě to umlčí, fajn.

h: Tu pozvánku budu ignorovat.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Každopádně. Facebook je na mě až moc. Potřebuji něco klidnějšího, méně úzkostného.

`hong({eyes:"neutral"});`

h: Co je nového na Twitteru?

`bb({eyes:"look"});`

[O né, koukej na tu strašnou novinku!](#act1d_news)

[O né, je ten tweet tajně o *nás*?](#act1d_subtweet)

[Hele, GIF kde kočka pije mléko.](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Bože, je to jak kdyby svět hořel, že?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Je ti jako by všechno končilo, jako by všechno umíralo a my jsme odsouzeni k zániku a nic s tím nenaděláme.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Pojďme retweetnout ten příběh!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Retweetnu to, ale prosím už mlč!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Do háje, tak se jdeme podívat na Snapchat.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: To je subtweet! Zákeřný, zákeřný subtweet!

`hong({eyes:"annoyed"});`

h: Ne, není?

`bb({eyes:"narrow", mouth:"small"});`

b: ale co když o nás všichni mluví za našimi zády

h: Ne, n--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: PŘED NAŠIMI ZÁDY

`hong({eyes:"sad", mouth:"sad"});`

h: Já s--

`bb({eyes:"narrow", mouth:"small"});`

b: ale *co když*

h: N--

`bb({eyes:"narrow_eyebrow"});`

b: *co když*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: o-KAY, zkusíme Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Heh jo to je roztomilé, zrovna jsme to retweetly, Myslí--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: KOČKY NESTRÁVÍ MLÉKO A MY JSME HROZNÍ LIDÉ, PROTOŽE SI UŽÍVÁME TÝRÁNÍ ZVÍŘAT

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: o-KAY, zkusíme Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Huh, fotky ze včerejší noci. Takže *takhle* ty týdení párty vypadají.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Uf, to vypadá na mou úzkost příliš přeplněně.

h: Možná jsem na tu pozvánku přecejen neměla říct ano?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Změnit naši odpověď? Jako hulvát?!](#act1e_yes_dontchange)

[Změň naši odpověď! Je tam až moc přeplněno!](#act1e_yes_changetono)

{{if _.subtweet}}
[Jo, subtweetovali nás.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Počkej, retweetli jsme to bez ověření faktů.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Víš že máš fakt špatné držení těla?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Spoléhali na to, že přijdeme, a teď my zrazujeme jejich důvěru? Chceme snad zemřít sami??!

{{if _.fifteencigs}}
b: PATNÁCT. CIGARET.
{{/if}}

{{if _.whalepoop}}
b: VELRYBÝ. TRUS.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Drž hubu, drž už hubu, nechám tam ano!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Nevíš o davovích panikách?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: V roce 2003 vypukl požár v nočním klubu na Rhode Islandu a panika donutila lidi zablokovat východy, takže 100 lidí uhořelo k smrti-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: CHCEŠ ABY SE NÁM TO STALO TAKY-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: ŘEKNI NE ŘEKNI NE ŘEKNI NE ŘEKNI NE ŘEKNI NE ŘEKNI NE ŘEKNI NE ŘEKNI NE ŘEKNI N-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Drž hubu, drž už hubu, změním to na ne! Bože!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... to vypadá celkem zábavně.

h: Možná jsme neměli odmítnout to pozvání?

`bb({mouth:"normal", eyes:"normal"});`

[Změnit naši odpověď? Jako hulvát?!](#act1e_no_dontchange)

[Změň naši odpověď! Neumři osamotě!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Jo, subtweetovali nás.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Počkej, retweetli jsme to bez ověření faktů.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Víš že máš fakt špatné držení těla?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Všichni s námi počítali!

b: ...nechat je na pokoji a dovolit jim užít si hezkou pařbu bez takového hrozného, nechutného podivína {{if _.whitebread}}a pojídače bílého chleba{{/if}} jako n--


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Drž hubu, drž už hubu, nechám tam ne!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Chronická osamělost zvyšuje hladinu kortizolu a také riziko kardiovaskulárních onemocnění a mrtvice!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: PATNÁCT. CIGARETT.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Drž hubu, drž už hubu, změním to na ano! Bože!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Všechny naše problematické tweety se vrátily nás strašit!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Obviní nás a zruší nás a potáhnou nás na laně přivázaném ke koni po informační dálnici!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Proč se takhle chováš?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Šíříme dezinformace! Ničíme důvěru ve svobodný tisk!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Jsme důvodem, proč z trosek demokracie povstane fašismus!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: Proč se takhle chováš?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Chceš mít preclík místo páteře?! Přestaň se hrbit nad obrazovkou!

```
bb({body:"meta"});
```

b: To znamená ty taky.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Proč se takhle chováš?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... to vypadá celkem zábavně.

h: Možná jsme tu pozvánku neměli ignorovat?

`bb({mouth:"normal", eyes:"normal"});`

[Ignorujte to dál, pořád by jsme zkazili večírek.](#act1e_ignore_continue)

[Vlastně, řekni ano.](#act1e_ignore_changetoyes)

[Vlastně, řekni ne.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: Je ale docela neslušné je pořád ignorovat, ne?

`bb({eyes:"normal_right"});`

b: No, ostatní lidé *nás* vždycky ignorují, takže-

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: Takže řekněme, že jsme si kvit.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Necháváš mě... se bavit?

b: No, myslím tím, že osamělost nás *může* zabít.
`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: Je tam moc lidí. Davy jsou nebezpečné.
(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: No nic. Nové oznámení na Tinderu.

`bb({eyes:"uncertain"})`

b: Co, ta seznamovací aplikace na jednorázovky? 

`hong({eyes:"annoyed"})`

h: Není to aplikace na jednorázovky, je to jen způsob, jak poznat nové lid--

`bb({eyes:"narrow"})`

b: Je to aplikace na jednorázovky.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Oh, mám shodu! Vypadají roztomile!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Prosím nezkaz mi t--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: NEBEZPEČÍ NEBEZPEČÍ NEBEZPEČÍ NEBEZPEČÍ NEBEZPEČÍ NEBEZPEČÍ

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Jsme *využíváni* jinými lidmi.](#act1f_used_by_others)

[Jenom *využíváme* ostatní lidi.](#act1f_using_others)

[TVŮJE SHODA JE SÉRIOVÝ VRAH](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Náhodné jednorázovky možná zaplní díru tam dole,

b: ale nikdy nezaplní tu díru...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *tady*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Jde o to, ŽE ZEMŘEME SAMI

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Myslíš si, že genitálie jiných lidí jsou Pokémoni, které můžeme sbírat?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (pokemon theme song)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ Chci být ta nej^děvka^řštější

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Jako nikdo jiný-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Stehna a zadek, vnadná prsa-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ s propoceným ^pérem^ a koulemi!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ PERVERT-MON! VŠECH-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Jde o to, že jsme manipulativní podivíni.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: Zavřou tě do studny a násilím tě budou krmit bílým chlebem, aby tě vykrmili a mohli nosit tvou kůži jako oblek!
{{/if}}

{{if _.parasite}}
b: Zmlátí tě pomodoro časovačem a řeknou: „MĚLS BÝT PRODUKTIVNĚJŠÍ, TY PARAZITE.“
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Roztrhají ti maso na krvavé konfety, z vnitřností udělají fáborky a z krve udělají punč!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Co říkáš na TOHLE pozvání na večírek?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: Tahle hra už mě tak nebaví.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"osamělost nás zabije"... {{/if}}
{{if _.parasite}}"jsme sociální parazit"... {{/if}}
{{if _.whitebread}}"nejes to, zabije nás to"... {{/if}}
{{if _.subtweet}}"mluví o nás za našimi zády"... {{/if}}
{{if _.badnews}}"svět hoří"... {{/if}}
{{if _.hookuphole}}"umřeme osamotě"... {{/if}}
{{if _.serialkiller}}"jsou sériový vrah"... {{/if}}
{{if _.catmilk}}"kočky nestráví mléko"... {{/if}}
{{if _.pokemon}}a ^crappy^ parody song... {{/if}}

h: Já chci jen žít svůj život.

h: já chci jen být volný/á od této... bolesti.

`bb({eyes:"look_sad"});`

b: Hej... člověče...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Bude to v pořádku.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Jako tvůj věrný hlídací vlk, Vždycky si budu dávat pozor na nebezpečí, a udělám vše pro to, aby jsme se uchránili.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Slibuju.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Poslední aplikace. Instagram. Co pro nás máš?

`hong({eyes:"sad"});`

h: Je to... víc fotek z té párty.

`hong({mouth:"sad"});`

h: Všichni vypadají tak šťastně. Bez obav. Bez úzkosti.

`hong({mouth:"anger"});`

h: Bože, proč nemůžu být jako oni? Proč nemůžu být prostě *normální*?

`bb({eyes:"normal_right"});`

b: Když už mluvíme o večírcích, ohledně pozvánek na tento víkend. Tady je mé KONEČNÉ rozhodnutí:

`bb({eyes:"normal"});`

[Měli bychom jít.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Neměli bychom jít.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "don't"`

(#act1h)

# act1h

b: My bych--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *^KURVA^.*

`hong({body:"2_you"});`

h: TY.

(...500)

b: c

(...1500)

`bb({eyes:"wat_2"});`

b: c- co?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Na tu párty řeknu ANO,
{{if _.act1g=="go"}}
h: NE protože to chceš ty, ale protože *já* to chci.
{{/if}}

{{if _.act1g=="dont"}}
h: Právě PROTOŽE to nechceš.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Ty mě NEkontroluješ.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: A teď mě omluv, zatímco si tady v zatracenym klidu sním tenhle lahodný sendvič.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[ÁÁÁÁÁ, UMŘEME](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[ÁÁÁÁÁ VŠICHNI NÁS NESNÁŠÍ](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[ÁÁÁÁÁ JSME STRAŠNÍ LIDÉ](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: ÁÁÁÁÁ UMŘEME ÁÁÁÁÁÁÁÁÁÁÁÁÁ

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: ÁÁÁÁÁ VŠICHNI NÁS NESNÁŠÍ ÁÁÁÁÁÁÁÁÁÁÁÁÁ

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: ÁÁÁÁÁ JSME STRAŠNÍ LIDÉ ÁÁÁÁÁÁÁÁÁÁÁÁÁ

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: GRATULUJI

(...500)

n: ÚSPĚŠNĚ JSTE OCHRÁNILI FYZICKÉ+SOCIÁLNÍ+MORÁLNÍ POTŘEBY SVÉHO ČLOVĚKA

n: PROČ, PODÍVEJTE SE, JAK JSOU VDĚČNÍ!

(...500)

n: NYNÍ, KDYŽ JE JEJÍ ENERGIE NA NULE, MŮŽETE PŘÍMO OVLÁDAT JEJÍ ČINNOST

`bb({mouth:"smile", eyes:"normal"});`

n: VYBERTE SI SVŮJ ZÁVĚREČNÝ TAH

`bb({mouth:"small_lock", eyes:"fear"});`

n: *DOKONČI JO*

[{BOJUJ: Potrestejte svůj stresující telefon!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{UTEČ: Schouli se do klubíčka a plač!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Tvůj telefonu ti vyvolal panický záchvat!

`bb({eyes:"anger"})`

b: Zuckerberg a spol. zneužívají tvoje duševní zdraví pro rizikové kapitalistické peníze!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Potrestej svůj telefon! Znič ho! Zabij ho!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: ZABIJ HO ZABIJ HO ZABIJ HO ZABIJ HO ZABIJ HO ZABIJ HO ZABIJ HO ZABIJ HO ZABIJ HO ZABIJ HO ZABIJ HO ZABIJ HO ZABIJ HO ZABIJ HO ZABIJ H--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Celý svět je plý nebezpečí!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Dělej jako pásovec! Schouli se do klubíčka pro sebeobranu!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: SCHOULI SE A BREČ SCHOULI SE A BREČ SCHOULI SE A BREČ SCHOULI SE A BREČ SCHOULI SE A BREČ SCHOULI SE A BR-- 

(#act1j)

# act1j

`SceneSetup.act1_outro()`
