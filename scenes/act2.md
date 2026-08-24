# act2

`SceneSetup.act2();`

{{if _.badnews && !_.factcheck}}
(#act2-preamble-news1)
{{/if}}

{{if _.badnews && _.factcheck}}
(#act2-preamble-news2)
{{/if}}

{{if _.catmilk}}
(#act2-preamble-cat)
{{/if}}

(#act2-preamble-tinder)


# act2-preamble-news1

```
publish("act2",["dee",3]);
```

s: Ale *viděla* jsi tu "zprávu" ohledně té strašné věci, která se stala někde?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: a-ahoj...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Boha. Já nesnáším zprávy. Je to jen o senzacích a clickbaitu.

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: h... hezká party...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Pravda, ale oni jednají jen popudově. Ten *reálný* problém je s lidmi, kteří klikají na clickbaity.

```
publish("act2",["dee",3]);
```

s: Kdo by retweetnul tak hrozný článek? Chce snad, aby se jeho kamarádi cítili špatně?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Uhhh, že jo?

(#act2-preamble-end)


# act2-preamble-news2

```
publish("act2",["dee",3]);
```

s: Ale *viděla* jsi, že ten "článek" je celkem virální?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: a-ahoj...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Jo, naprosto falešný. Kdo by tomu věřil a ještě to retweetnul?

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: h... hezká party...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Vážně kámo. Jako fakt? Co takhle otevřít Google a ověřit si fakta?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Uhhh, že jo?

(#act2-preamble-end)


# act2-preamble-cat

```
publish("act2",["dee",3]);
```

s: Jak jsem říkala, mašinérie na memy zneužívá kočky.

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: a-ahoj...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Rozeber tu myšlenku trochu.

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: h... hezká party...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Víš, viděla jsem včera někoho retweetnout GIF kočky, co pije mléko.

```
publish("act2",["dee",3]);
```

s: Nemůžou ten ^kekel^ trávit! Kdo by takhle retweetoval *zneužívání zvířat*?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Uhhh, že jo?

(#act2-preamble-end)


# act2-preamble-tinder

```
publish("act2",["dee",1]);
```

s: No a žádná odpověď už nepřišla.

```
publish("act2",["dee",0]);
publish("act2",["party_hong","next"]);
```

h2: a-ahoj...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: I přesto, že máte oba match na Tinderu?

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: h... hezká party...

```
publish("act2",["party_hong","next"]);
```

{{if _.serialkiller}}
(#act2-preamble-serialkiller)
{{/if}}

{{if _.hookuphole}}
(#act2-preamble-hookuphole)
{{/if}}

{{if _.pokemon}}
(#act2-preamble-pokemon)
{{/if}}

# act2-preamble-serialkiller

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Já ti nevím. Třeba si myslel, že jsem *sériový vrah* nebo co? Tak paranoidní.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Uhhh, že jo?

(#act2-preamble-end)


# act2-preamble-hookuphole

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Já ti nevím. Třeba si myslí, že jednorázovky nezaplní tu díru v jejich životě?

s: Nebuď taková pruda! Otevři svou mysl, pak rozhoď nohy!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Uhhh, že jo?

(#act2-preamble-end)


# act2-preamble-pokemon

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Já ti nevím. Nebyl tak sexy, ale byl by fakt dobrý úlovek.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: CHYŤ JE VŠECHNY!™ 

(#act2-preamble-end)

# act2-preamble-end

```
Game.clearText();
publish("act2-out-1");
music(null, {fade:1});
```

(...3000)

```
music('battle', {volume:0.5});
publish("hp_show");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

n: DRUHÉ KOLO: *BOJUJTE!*

[Ale ne, všichni nás nenávidí!](#act2a_social)

[*Nezíráš* náhodou na tu zrzku?](#act2a_perv)

[Hej, pojďme se pobavit o smyslu života.](#act2a_meaning)

# act2a_social

`bb({eyes:"sad"})`

b: Kazíme náladu na celé párty tím, že jsme takový smutný ^zaprděnec^!

`bb({eyes:"shock", body:"two_up"})`

b: Zabíjíme tady tu dobrou atmosféru! Právě pácháme atmo-vraždu první kategorie!

`bb({eyes:"normal", body:"normal"})`

b: Člověče, musíme *teď* odejít, než--

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: Je hezčí než my, což znamená, že jestli se na ní *podíváme*, tak--

`bb({eyes:"shock", body:"two_up"})`

b: JSME ÚCHYLÁCI

`bb({body:"normal"})`

b: Jsme úchylní, zlí, špatní špatní špatní hrozní hrozní úchy--

```
_.a2_first_danger = 'perv';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2a_meaning

`bb({body:"one_up", eyes:"normal_r"})`

b: Konec konců, co zásadního můžeme udělat?

`bb({body:"normal", eyes:"sad"})`

b: Přispět lidstvu? Všechna velká díla se rozpadnou jak Kytice. Láska? Smrt nás vždy rozdělí.

`bb({eyes:"sad_r"})`

b: A kolik je na světě smrti! *My* umřeme. *Naši milovaní* umřou.

`bb({eyes:"shock", body:"two_up"})`

b: Sakra, druhý termodynamický zákon říká, že *vesmír* umře!

`bb({eyes:"suspect", body:"normal"})`

b: A, že "smrt nás nutí cenit si života"? To je jako říkat, že otroctví je super, jelikož doceníš svobodu!

`bb({body:"one_up"})`

b: A, že "si musíš udělat vlastní smysl života"? To je přesně, co kultisti a konspirační teoretici dělají!

`bb({eyes:"shock", body:"two_up"})`

b: Život nemá smysl, smrt nemá smysl, ani *smysl* nemá smysl! Co smrtelná duše vlas--

```
_.a2_first_danger = 'meaning';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2b

`bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"suspect"})`

b: Uhh... vidíš mě, člověče?

`bb({eyes:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"shock", mouth:"small_talk", body:"chest", MOUTH_LOCK:true})`

b: *NÁDECH*

`bb({mouth:"small_talk"})`

b: MUSÍM TĚ VAROVAT...

[*Více* toho samého nebezpečí!](#act2b_louder)

{{if _.a2_first_danger=="social"}}
[*Jiné* společenské nebezpečí!](#act2b_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[*Jiné* morální nebezpečí!](#act2b_different_moral)
{{/if}}

[Ignoruješ nebezpečí! To je nebezpečné!](#act2b_ignore)

# act2b_louder

`_.a2_first_choice = "louder"`

{{if _.a2_first_danger=="social"}}
(#act2b_louder_social)
{{/if}}

{{if _.a2_first_danger=="perv"}}
(#act2b_louder_perv)
{{/if}}

{{if _.a2_first_danger=="meaning"}}
(#act2b_louder_meaning)
{{/if}}

# act2b_louder_social

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: EMOCE JSOU NAKAŽLIVÉ! TAKŽE POKUD NEODEJDEŠ, TAK NAKAZÍŠ NĚKOHO SVOU MENTÁLNÍ NEMOCÍ! 

b: Způsobíš epidemii SMUTNÉHO ^ZAPRDĚNCE^

`bb({eyes:"suspect", body:"normal", mouth:"normal"})`

b: Musíme vypadnout a jít do karantény v malé místnosti s Netflixem a dovážkou jídla!

```
_.a2_second_danger = 'netflix';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "karanténa";
```

(#act2c)

# act2b_louder_perv

`bb({eyes:"suspect", body:"two_up", mouth:"normal"})`

b: NEBUĎ ÚCHYL. JE TO PROTIZÁKONNÉ!

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: Proti-úchylný zákon č. 152/2021 Sb.: (1) Kdokoliv, kdo koukne na (a) ta nasvalená ramena (b) tu oblou zadnici (2) bude znám jako

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: "VELKÝ NECHUTNÝ HNUSNÝ ÚCHYL"

```
_.a2_second_danger = 'law';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "zákon";
```

(#act2c)

# act2b_louder_meaning

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: Vlastně, i když najdeme smysl života, tak *stále* můžeme všechno pokazit!

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Alfred Nobel chtěl světový mír a aby si kultury rozuměly. Tak se rozhodl, že zjednoduší cestování.

`bb({eyes:"normal_r"})`

b: Což vyžadovalo způsob, jak jednoduše hloubit tunely. Tak vynalezl nový materiál zvaný "dynamit"...

`bb({body:"one_up", eyes:"normal"})`

b: který použili v první světové, aby ZABILI MILIÓNY LIDÍ

`bb({body:"two_up", eyes:"shock"})`

b: JE TO EFEKT MOTÝLÍCH KŘÍDEL! KOLIK LIDÍ OMYLEM ZABÍJÍŠ PRÁVĚ TEĎ

```
_.a2_second_danger = 'butterfly';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "první světová válka";
```

(#act2c)

# act2b_different_social

`_.a2_first_choice = "different"`

`bb({eyes:"normal_r", body:"point", mouth:"normal"})`

b: Víš, co je horší než, když tě nemá nikdo rád? Když tě mají *všichni* rádi.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: No jo, stát se jedním z *těch* požitkářských večírkových pařmenů.

`bb({body:"normal", mouth:"small"})`

b: Povrchní život s povrchními přáteli, kteří znají tvé povrchní já.

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Člověče, musíme utéct od těchto požitkářských zombíků, než nás přemění na jednoho z nich!

```
_.a2_second_danger = 'zombies';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "zombíci";
```

(#act2c)

# act2b_different_moral

`_.a2_first_choice = "different"`

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Celé rodiny umírají v genocidách *právě teď* a my tu paříme!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Moudrý člověk jednou řekl, "Jediné, co je nezbytné pro triumf zla, je, aby dobří lidé nic nedělali"

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: MY NIC NEDĚLÁME.

`bb({mouth:"small"})`

b: PAŘENÍM POMÁHÁME *HITLEROVI*.

```
_.a2_second_danger = 'hitler';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "Hitler";
```

(#act2c)

# act2b_ignore

`_.a2_first_choice = "ignore"`

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Myslíš si, že jsi v bezpečí, jelikož jsi jen vyndala baterky z hlásiče oxidu uhelnatého.

`bb({eyes:"suspect_r"})`

b: Ani ten jed neucitíš! Jen usneš a pak--

`bb({body:"scream_c_1"})`

b: UMŘEEEEEEEEEEŠ

```
_.a2_second_danger = 'ignore';
_.a2_attack_2 = "harm";
_.a2_hoodie_callback = "oxid uhelnatý";
```

(#act2c)

# act2c

```
hong({body:"ignore_sweat"});
bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true});
```

b: ...

`bb({eyes:"happy", mouth:"smile", body:"chest"})`

b: Díky bohu, myslím, že mě znovu slyšíš!

`bb({eyes:"closed", body:"point"})`

b: MUSÍM TĚ VAROVAT O...

{{if _.a2_first_choice=="louder"}}
[*Ještě více* toho samého nebezpečí!](#act2c_louder)
{{/if}}

{{if _.a2_first_choice!="louder"}}
[*Více* toho samého nebezpečí!](#act2c_louder)
{{/if}}

{{if _.a2_first_danger=="social"}}
[*Jiné* společenské nebezpečí!](#act2c_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[*Jiné* morální nebezpečí!](#act2c_different_moral)
{{/if}}

[Zkontrolovala jsi ten punč, který pijem?](#act2c_punch)

#act2c_louder

{{if _.a2_second_danger=="netflix"}}
(#act2c_louder_netflix)
{{/if}}

{{if _.a2_second_danger=="law"}}
(#act2c_louder_law)
{{/if}}

{{if _.a2_second_danger=="butterfly"}}
(#act2c_louder_butterfly)
{{/if}}

{{if _.a2_second_danger=="zombies"}}
(#act2c_louder_zombies)
{{/if}}

{{if _.a2_second_danger=="hitler"}}
(#act2c_louder_hitler)
{{/if}}

{{if _.a2_second_danger=="ignore"}}
(#act2c_louder_ignore)
{{/if}}

# act2c_louder_netflix

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: Ve skutečnosti, Netflix a dovážka jídla není dostatečná karanténa! Stále bychom nakazili poslíčka!

`bb({body:"one_up", mouth:"small"})`

b: Musíme se přesunout někam do Finska za polární kruh a mít jídlo dovážené dronem!

`bb({body:"two_up", mouth:"normal"})`

b: A ještě by museli dezinfikovat ten dron kvůli našim virům SMUTNÉHO ZAPRDĚNCE

`_.a2_attack_3 = "alone";`

`_.a2_hoodie_callback = "karanténa";`

(#act2d)

# act2c_louder_law

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: VELKÝ NECHUTNÝ HNUSNÝ ÚCHYL bude odsouzen na 72 hodin v jednom z těch středověkých zařízení na veřejné ponížení

b: pokud to tedy není *jejich záliba*

`bb({body:"scream_a_1"})`

b: protože je VELKÝ NECHUTNÝ HNUSNÝ ÚCHYL

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "zákon";`

(#act2d)

# act2c_louder_butterfly

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: EFEKT MOTÝLÍCH KŘÍDEL! Používáš nerozložitelný kelímek?

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: BUM, SKLÁDKA VYPUSTÍ JED A ZABIJE DÍTĚ

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: Potíš se a buší ti srdce?

`bb({body:"scream_a_1"})`

b: BUM, ZBANKROTOVALA JSI NAŠE ZDRAVOTNICTVÍ A MILIONY UMŘOU

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "efekt motýlích křídel";`

(#act2d)

# act2c_louder_zombies

`bb({body:"normal", mouth:"small", eyes:"angry"})`

b: Tihle požitkářští zombíci přijdou k tobě mumlající,

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: LIIIIIKE. LIIIIIIIIIIKE.

`bb({body:"scream_a_1"})`

b: Kousnou tě a promění tě do BEZMOZKOVÉHO TÝPKA či NEPŘEMÝŠLEJÍCÍ PIPKY

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "zombíci";`

(#act2d)

# act2c_louder_hitler

`bb({body:"scream_a_1"})`

b: NACISTI PRÁVĚ TĚĎ ZASE POCHODUJÍ NA ULICÍCH

`bb({body:"one_up", mouth:"smile", eyes:"happy"})`

b: Říkat, *ještě že 'dobří lidé' se poflakovali 'relaxováním' a 'self-care'!*

`bb({body:"point", mouth:"smile", eyes:"happy_r"})`

b: *Náš plán je jít kupředu, ani krok zpátky!*

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "Hitler";`

(#act2d)

# act2c_louder_ignore

`bb({body:"normal", mouth:"normal", eyes:"normal_r"})`

b: Zamysli se nad tím, víme, zda tato budova *má* detektory oxidu uhelnatého?!

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: Co když se trávíme *PRÁVĚ TEĎ?*

`bb({body:"scream_a_1"})`

b: ANI BYCHOM NEVIDĚLI SMRT PŘICHÁZET. PROSTĚ BYCHOM PŘESTALI EXISTOVAT NAVĚKY A NAVŽDY A NA--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "oxid uhelnatý";`

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: Co když jsme *absolutně neschopní* být milováni, nebo milovat ostatní?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: Co když se něco nevratně rozbilo uvnitř nás dlouho zpátky? Nebo to nikdy neexistovalo?

`bb({body:"scream_a_1"})`

b: AHH JSME ROZBITÍ! TAK ROZBITÍ TAK ROZBITÍ TAK ROZB--

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Co když jsme *zhnilí zevnitř?*

`bb({body:"one_up", eyes:"sad"})`

b: Ostatní mají vlastní chuť dělat dobré věci, ale my děláme "dobré věci" jen kvůli pocitu viny či studu, pokud vůbec.

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: Co když naše nátura ublíží ostatním? Co když nezvládneme být *něčím jiným* než přítěží pro ty kolem nás?

`bb({body:"scream_a_1"})`

b: AHH JSME ROZBITÍ! TAK ROZBITÍ TAK ROZBITÍ TAK ROZB--

`_.a2_attack_3 = "bad";`

(#act2d)

# act2c_punch

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Já nejsem iracionální. Lidé *dělají* drogové punčové údery. To je reálná věc, co se reálně děje.

`bb({eyes:"suspect"})`

b: Člověče, bolí tě hlava? Jsou tvé končetiny ochablé? Myslím, že umíráme.

`bb({body:"scream_a_1"})`

b: AHHH MY UMÍRÁME! MY UMÍRÁME MY UMÍRÁME MY UMÍR--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "punčové údery";`

(#act2d)

# act2d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"attacked"});
attack("20p", _.a2_attack_1);
```

(...401)

```
hong({body:"attacked_2"});
attack("20p", _.a2_attack_2);
```

(...401)

```
hong({body:"attacked_3"});
attack("20p", _.a2_attack_3);
```

(...1001)

h: K^RVAAA^!

h: ZK^URVENÝ^ K^URVY^ K^KUREV^SKÝ *K^URVA^*

`bb({body:"two_up", mouth:"smile", eyes:"happy"});`

b: Jéj, člověče! Jsem tak rád, že mě zase slyšíš!

`bb({body:"normal", mouth:"small", eyes:"sad"})`

b: Proč jsi mě ignorovala?

`hong({body:"facepalm"})`

h: Ach jo, ty jeden hlupáčku.

`hong({body:"facepalm_2"})`

h: Znáš ten příběh od původních Američanů?

h: "Uvnitř tebe jsou dva vlci: jeden je naděje, druhý je zoufalství. Který z nich vyhraje? Ten, kterého krmíš."

```
hong({body:"facepalm_3"});
bb({eyes:"normal"});
```

h: Snažila jsem se tě *vyhladovět*. Ty sadistický ^zmetku^!

`hong({body:"smile", mouth:"smile"})`

h: Kašlu na to. Zkusím pozitivní myšlení.

h: *Jsem milovaná. Jsem dobrá. Jsem chytrá. Jsem krásná. Jsem speciální.*

`bb({eyes:"suspect"});`

[Sakryš, ty jsi ale narcis.](#act2d_narcissist)

[Víš, že pozitivní myšlení bylo *vyvráceno?*](#act2d_disproven)

[omg nemůžeš připisovat náhodné příběhy domorodcům](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Ve skutečnosti se to u lidí s malým sebevědomím vždy *obrátí* proti nim! 

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: Byla to dobře navržená studie. Randomizovaná kontrolovaná studie. Byl to dvojitě zaslepený experiment, takže vědec nevěděl, jaká skupina je jaká.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Výsledek: pokud máš nízké sebevědomí, snažit se o pozitivní myšlení tvé myšlení ovlivní *hůře*, než kdybys nedělala nic.

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Wood 2009, Psychological Science. Najdi si to na Google Scholar, člověče

`bb({body:"scream_b_1"})`

b: A PŘESTAŇ ŠÍŘIT NEVĚDECKÉ DESINFORMACE

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_narcissist

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: *Musíš* pokorně příjmout své chyby aby ses stala lepším člověkem!

`bb({body:"two_up", eyes:"suspect"})`

b: Nemůžeš použít osvěžovač vzduchu na plesnivou místnost! Zametat své chyby pod koberec tě v dlouhodobém hledisku zkazí.

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: Naštěstí, já, tvůj věrný hlídací pes, tě vždy upozorním na tvé chyby. A právě teď, je-

`bb({body:"scream_b_1"})`

b: VŠECKO. VŠECIČKO ŠPATNĚ

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Původní Američané jsou *reální lidé*, ne nějací "povznešení divoší", které můžeš zmínit, abys své rady z horoskopu udělala více *exotická*.

`bb({eyes:"suspect_r"})`

b: Ty redukuješ individua a komplexní kultury do nápisu na kartičce se přáním! To je "benevolentní rasismus"!

`bb({body:"scream_b_1"})`

b: PŘESTAŇ BÝT RASISTA TY ŠILHAVÝ HRUBIÁNE

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2e

h: DO ^PRDELE^.

`hong({body:"yell", mouth:"yell"})`

h: Víš co? Jsi *iracionální*.

h: Každý ví, že emoce jsou iracionální! Obvzláště strach!

`hong({body:"facepalm_2"})`

h: Jsi jen neužitečný pozůstatek evoluce, jako slepé střevo nebo zub moudrosti!

`hong({body:"yell", mouth:"yell"})`

h: ^Kruci^, tahle celá vlční metafora je stupidní! Ty jsi jen hromada neurotransmiterů v mojí hlavě.

`hong({body:"cross", mouth:"cross"})`

h: Proč bych měla poslouchat takové bezcenný, iracionální, neexistující kus ^hovna^, jako jsi ty?!

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Sakra, člověče. To mě fakt ranilo.](#act2e_hurtful)

[Jsem pocit, pocity jsou validní.](#act2e_valid)

[Člověče, my jsme *oba* "jen chemikálie."](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: Jsem *část* tebe, víš. Když to říkáš, tak jen ubližuješ sama *sobě*.

`bb({body:"scream_a_1"})`

b: Proč si ubližuješ, člověče? PŘESTAŇ SI UBLIŽOVAT.

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2e_rational

`bb({body:"normal", mouth:"normal", eyes:"normal_r"});`

b: Tvá nejnitěrněší motivace je dopamin, tvá největší radost je serotonin.

`bb({body:"one_up"});`

b: Tvé vzpomínky jsou jen synaptické váhy, tvé uvažování jsou jen poruchové elekrické signály.

`bb({eyes:"normal", body:"normal"});`

b: Takže pokud to, že jsem "jen chemikálie" znamená, že *jsem* iracionální... tak to znamená, že i "ty jsi" iracionální!

`bb({body:"two_up", eyes:"shock"});`

b: A pokud jsme *oba* iracionální, tak *nikdy* nepříjdeme na to jak žít šťastný a naplněný život.

`bb({body:"scream_a_1"})`

b: AHHH JSME ROZBITÍ! TAK ROZBITÍ TAK ROZBITÍ--

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2f)

# act2e_valid

`bb({body:"normal", mouth:"normal", eyes:"suspect"});`

b: Počkej... "oni" říkají, že pocity jsou validní, že bys měla vždy příjmout své emoce.

`bb({eyes:"suspect_r"});`

b: Ale "oni" také říkají, že emoce jsou iracionální, že emocím se nedá věřit.

`bb({eyes:"angry"});`

b: Ó můj bože, "oni" nám celou tu dobu lhali!

`bb({body:"scream_a_1"})`

b: "ONI" NÁM PŘEDHAZOVALI NAVZÁJEM ROZPORUJÍCÍ SE INFORMACIE, ABY NÁS UDĚLALI ZÁVYSLÝMI NA SELF-HELP PRŮMYSLU

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2f

`hong({body:"defeated", MOUTH_LOCK:true});`

h: ...

h: Nesnášim to. Bože to bolí tak moc, já tohle *nesnáším*.

h: Nemůžu tě nijak upokojit. Nemůžu tě ignorovat. Nemůžu s tebou bojovat.

`bb({eyes:"suspect"});`

h: Ať dělám, co dělám, nemůžu se tě zba-

`bb({body:"cry_1"});`

b: Možna, ty se máš *ZBAVIT* mě.

`bb({body:"cry_2"});`

b: Jak si myslíš, že se cítím *já*, člověče?!

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: Já se snažím být tvým ochraným psem, ale ty mě stále vidíš jako nějakého velkého zlého vlka!

b: Takže já se budu snažit ještě *víc* abych tě varoval na nebezpečí! *Více* nebezpečí! *Nejrůznější* nebezpečí!

`bb({eyes:"cry_2"})`

b: Ale bez ohledu na to, jak moc se snažím tě chránit, ty si *stále* myslíš, že jsem tvůj nepřítel!

`bb({body:"cry_5"});`

b: Co dělám špatně?!

`bb({body:"cry_2"});`

b: Já *vím*, že mi to moc nejde, ale já se *snažím*, člověče!

`bb({body:"cry_3"});`

b: ...já se snažím.

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: Nemusíš dbát na mé varování, nebo se mnou souhlasit, či mě mít *ráda*.

`bb({eyes:"cry_r_2"});`

b: Já jen... jediné co chci je, abys byla se mnou trpělivá.

`bb({eyes:"cry_r_3"});`

b: Já jen chci, aby sis sedla se mnou chvilku, místo otáčení se ke mě zády a--

```
bb({eyes:"cry_r_4"});
hong({body:"listen"});
```

r: Hej.

```
hong({body:"look"});
Game.clearText();
publish("act2-in-2");
publish("hp_hide");
music('party1', {volume:0.4, fade:2});
```

(...2000)

```
publish("act2",["party_hunter",2]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Vypadá to, že jsem tě chytnul ve vnitřním boji, špunte.

```
publish("act2",["party_hunter",3]);
publish("act2",["party_hong",13]);
```

h2: Bylo to tak očividné?

```
publish("act2",["party_hunter",4]);
publish("act2",["party_hong",14]);
```

r: Ty jsi, ah, mumlala na svou mikinu ohledně {{_.a2_hoodie_callback}} nebo něco takového.

```
publish("act2",["party_hunter",13]);
publish("act2",["party_hong",15]);
sfx("rustle", {volume:0.6});
setTimeout(function(){
	publish("act2",["party_hong",16]);
	sfx("concrete_step3", {volume:0.6});
},401);
setTimeout(function(){
	publish("act2",["party_hong",17]);
	sfx("concrete_step4", {volume:0.6});
},801);
```

h2: Ah bože já jsem taková ^kráva^.

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Hej. Nejsi sama, kamarádko. Úzkost je mega běžná.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r: Kruci, třeba včera, jsem slyšel, jak se někdo na kampusu nervově zhroutil a rozmlátil si svůj telefon!
{{/if}}

{{if _.act1_ending=="flight"}}
r: Kruci, třeba včera, jsem slyšel, že se někdo schoulil jak pásovec a na veřejnosti se rozplakal!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Poslouchej: Já vím, jaké to je mít to zvíře v hlavě.

```
publish("act2",["party_hunter",8]);
```

r: My *všichni* ho máme. To je důvod, proč dělám každý víkend party, aby se zapomělo na trable, zapomělo na to zvíře.

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: ale moje úzkost...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: Žádný strach, špunte. Býval jsem jako ty. Pak jsem ale objevil menší trik jak ten negativní hlas umlčet na vždy...

```
publish("act2",["party_hunter",3]);
Game.clearText();
music(null, {fade:1});
```

(...2001)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",22]);
sfx("rustle");
```

(...2501)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",23]);
sfx("rustle2");
```

(...1001)

```
publish("act2",["party_hunter",11]);
```

r: Můj vlastní osobní mix. Je trochu silnější než... no, vlastně cokoliv legálního.

```
publish("act2",["party_hunter",12]);
publish("act2",["party_hong",24]);
```

r: Do dna, ^ču-bíno^!

```
hong({body:"hold"});
bb({body:"normal", mouth:"small", eyes:"wat"});
Game.clearText();
Game.WORDS_HEIGHT_BOTTOM = -1;
publish("act2-out-3");
publish("hp_show");
```

(...3500)

[O můj bože.](#act2g_1) `Game.OVERRIDE_CHOICE_LINE=true`

[Tohle je špatný coping mechanismus.](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

[Neber si pití od cizích lidí.](#act2g_3) `Game.OVERRIDE_CHOICE_LINE=true`

# act2g_1

b: O--

(#act2g)

# act2g_2

b: T--

(#act2g)

# act2g_3

b: N--

(#act2g)

# act2g

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"forward", mouth:"forward"});
bb({body:"frazzled", mouth:"frazzled", eyes:"frazzled"});
```

h: Hmmm, jaká unikátní chuťová paleta!

h: Taková plnotučná příchuť "umlč svou mysl," s lehkým ocasem z "nikdy už nechci nic cítit"!

b: Tohle je špatné, člověče. Tohle je fakt, fakt špatné.

[Tohle je *přesně* jak závislost začíná.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[Já *vědel*, že s tím pozváním bylo něco špatně!](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[Víš, že do toho mohl něco hodit?!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`


# act2h_opt1

b: Tohle je *pes*--

(#act2h)

# act2h_opt2

b: Víš, že do to --

(#act2h)

# act2h_opt3

b: Víš, že do to--

(#act2h)

# act2h

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"back", mouth:"back"});
bb({body:"panicked", mouth:"panicked", eyes:"panicked"});
```

h: Výborné *a* levnější než terapie!

b: ČLOVĚČE PROSÍM PŘESTAŇ

h: Hehehe!

h: A co s tím *ty* uděláš, ^kreténe^?

b: Já se ti omlouvám, člověče.

b: Já budu muset použít můj SPECIÁLNÍ ÚTOK

```
bb({body:"special_a"});
music('battle', {volume:0.5});
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act2h_attack) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act2h_attack) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act2h_attack) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`

# act2h_attack

```
bb({body:"special_b_1"});
hong({body:"forward", mouth:"forward"});
sfx("charging");
```

h: Co je to za ^sračku^?

h: Ty budeš tlachat víc stupidních *slovíček* mým směrem, aby--

```
bb({body:"special_c"});
sfx("hadouken");
```

(...901)

(#act2i)

# act2i

```
publish("hide_tabs");
publish("show_special_attack");
Game.FORCE_CANT_SKIP = true;
music(null);
stopAllSounds();
```

(...5000)

```
publish("show_tabs");
hong({ body:"final", mouth:"final" });
bb({ body:"normal", mouth:"normal", eyes:"sad" });
attack("100p", _.SPECIAL_ATTACK);
Game.FORCE_CANT_SKIP = false;
setTimeout(function(){
	publish("remove_special_attack");
},30);
```

(...2500)

h: CO TO ^KURVA^ BYLO

b: Já se omlouvám. Musel jsem ti ukázat následky.

{{if _.SPECIAL_ATTACK=="harm"}}
h: MOHLA JSEM *VIDĚT* MOJÍ VLASTNÍ MRTVOLU. MOHLA JSEM *CÍTIT*, JAKÉ JE TO BÝT SKUTEČNÉ MRTVÁ.
{{/if}}

{{if _.SPECIAL_ATTACK=="alone"}}
h: MOHLA JSEM *VIDĚT* VŠECHNY TY ZNECHUCENÉ POHLEDY. MOHLA JSEM *SLYŠET* VŠECHNY TY DRBY CO ŘÍKALI.
{{/if}}

{{if _.SPECIAL_ATTACK=="bad"}}
h: MOHLA JSEM *SLYŠET* DRCENÍ ŽEBER. MOHLA JSEM *CÍTIT* KREV VE VZDUCHU.
{{/if}}

b: Promiň, člověče.

n: *UKONČI TO*

[{BOJUJ: Dej pěstí hostiteli.}](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[{UTEČ: Jdeme pryč.}](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: Ten psychouš tě zneužívá.

b: Snaží se tě zkazit, udělat tě stejně narušenou, jako je on!

`bb({ body:"yell_angry_1" });`

b: Dej mu pěstí! Dej mu absolutního vypínáka!

`bb({ body:"final_1" });`

b: PRAŠŤ HO PRAŠŤ HO PRAŠŤ HO PRAŠŤ HO PRAŠŤ HO PRAŠŤ HO PRAŠŤ HO PRAŠŤ HO PRAŠŤ HO PRAŠŤ HO PRAŠŤ HO PRA--

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: Já *věděl*, že tihle pařmeni jsou hluboce narušená individua. Všichni utlumují své trable hroznými věcmi!

`bb({ body:"yell_1" });`

b: A tebe přesvědčují, abys dělala to samé! Kazí tě! Musíme vypadnout!

`bb({ body:"final_1" });`

b: VYPADNOUT VYPADNOUT VYPADNOUT VYPADNOUT VYPADNOUT VYPA--

`_.a2_ending = "flight";`

(#act2k)

# act2k

```
Game.clearText();
publish("act2-in-4");
publish("hp_hide");
music('party1', {volume:0.6, fade:1.5});
```

(...2001)

```
publish("act2",["party_hong",26]);
sfx("slide");
```

(...1001)

```
publish("act2",["party_hunter",14]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Jsi v poho, špunte?

`publish("act2",["party_hunter",13]);`

{{if _.a2_ending=="fight"}}
(#act2k_fight)
{{/if}}

{{if _.a2_ending=="flight"}}
(#act2k_flight)
{{/if}}

# act2k_fight

```
Game.clearText();
publish("act2",["party_hunter",21]);
publish("act2",["party_hong",33]);
music(null);
sfx("hit");
```

(...1000)

```
sfx("record_scratch");
publish("act2",["party_hunter",22]);
publish("act2",["party_hong",34]);
publish("act2",["dee",6]);
publish("act2",["dum",6]);
```

r: T-ty...

```
publish("act2",["party_hunter",23]);
publish("act2",["party_hong",35]);
publish("act2",["dee",5]);
publish("act2",["dum",5]);
music('party1', {volume:0.6, fade:6});
```

r: jsi *kinky*.

r: To se mi líbí. Přijď na párty příští víkend, cukrouši.

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: ok, čau, ciao, adios, au revoir, bye

r: To zvíře možná vyhrálo dneska, ale přijď zpět, a já ti namíchám něco ještě něco silnějšího!

h2: sayōnara, auf wiedersehen, zài jiàn, shalom

r: Ty a já, špunte, my ukážeme tomu zvířeti, kdo je šéf!

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h2: ok promiň, musím běžet

`publish("act2",["party_hunter",16]);`

r: ^Sakra^. To zvíře dnes vyhrálo, co?

`publish("act2",["party_hunter",15]);`

h2: ne ne, jen, hmmm, musím dát maraton. musím běžet.

`publish("act2",["party_hunter",19]);`

r: Přijď na mojí party příští víkend, cukrouší. Namíchám něco ještě něco silnějšího.

h2: ok, díky musím běžet běžet běžet běžet

r: Ty a já, špunte, my ukážeme tomu zvířeti, kdo je šéf!

(#act2k_end)

# act2k_end

```
Game.clearText();
publish("act2-out-5");
publish("act2-outro", ["end1"]);
music("hum", {fade:2, volume:0.6});
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2500)

```
publish("act2", ["act2_end",2]);
sfx("whoosh");
```

(...1000)

b: Člověče! Jsi v pohodě?!

```
publish("act2", ["act2_end","next"]);
```

b: Jéžiš, to bylo *těsné.* Vážně jsme mohli--

```
Game.clearText();
publish("act2", ["act2_end","next"]);
music(null);
sfx("squeak");
```

(...1500)

```
publish("act2", ["act2_end","next"]);
sfx("hit");
```

(...1000)

h: Já na tu párty jdu znova příští víkend.

h: Přiště, až budeme spolu bojovat, nejen že tě *porazím*...

h: Já tě ^kurva^ *zabiju*.

```
Game.clearText();
publish("act2", ["act2_end","next"]);
sfx("concrete_step1");
````

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step2", {volume:0.8});
```

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step3", {volume:0.5});
```

(...901)

`sfx("concrete_step4", {volume:0.25});`

(...3000)

`_.INTERMISSION_STAGE = 2;`

(#intermission)