# Hugmyndir að verkefni





## Hugmynd 1 - Tilmælavél og meðmælakerfi / Recommendation Engine and Recommendation System
### Notandi
Leikjaspilarar sem eru búnir að klára leik sem þeim þótti frábær og vilja finna næsta leik til að spila án þess að eyða mörgum klukkustundum í að leita.

### Vandamál
Leysir valkvíða (choice paralysis). Í stað þess að leita í gegnum 13.000+ leiki fær notandinn ábendingar byggðar á tölfræðilegum líkindum og einkunnum.

### Gögn sem hugmyndin notar
genre, rating_score_pct, developer, images (screenshots, cover_image_path)

### Aðalflæði
1. Notandinn slær inn eða velur leik sem hann heldur upp á (t.d. Castlevania: Symphony of the Night).
2. Kerfið greinir einkenni leiksins (genre, developer, decade).
3. Tilmælavélin reiknar út og birtir topp 5 leiki sem líkjast valda leiknum og hafa háa einkunn (rating_score_pct).
4. Notandinn getur smellið á meðmælin til að skoða screenshots, description og rating.

### Af hverju gæti þetta verið gott verkefni?
Það leysir raunverulegt vandamál hjá spilurum og nýtir einkunnir og flokkunargögn í svokallaða rökrétta virkni frekar en bara flata leit.

### Helstu áhættur
Að hanna einkunnagjafar- og líkindaalgoritmann þannig að hann mæli með réttum leikjum (t.d. að vega saman genre og rating_score_pct á réttan hátt).







## Hugmynd 2 - Retro Time Machine & Console Wars
### Notandi
Leikjasögunörðar og nostalgíuleitendur sem vilja kanna ólík tímabil tölvuleikjasögunnar eða bera saman samkeppnisaðila á leikjamarkaðnum.

### Vandamál
Gerir söguleg tölvuleikjagögn lifandi og sjónræn í stað flatrar leitar. Leysir skort á uppgötvun á óþekktum leikjum með því að breyta leit í gagnvirkt tímaferðalag og handahófskennda uppgötvun (random discovery).

### Gögn sem hugmyndin notar
platform_generation, decade, rom_size_mb, developer, box3d_path, screenshots

### Aðalflæði
1. Notandinn velur tímabil eða console wars (t.d. 16-bita tímabilið: SEGA Genesis vs. Super Nintendo).
2. Kerfið birtir gagnvirka tímalínu og samanburð á skráarstærðum leikja (rom_size_mb), rating og yfirburðum developer / publisher.
3. Notandinn ýtir á „Time Warp / Slot Machine“ hnappinn til að fá random discovery.
4. Kerfið dregur fram faldan gæðaleik frá því tímabili ásamt 3D box (box3d_path), screenshots og developer sögu.

### Af hverju gæti þetta verið gott verkefni?
Mjög skapandi og skemmtileg nálgun á gögnin sem nýtir stærð skráa (rom_size) og 3D kápumyndir á hátt sem flest venjuleg leikjasöfn gera ekki.

### Helstu áhættur
Að hanna myndræna tímalínu og taka saman tölfræðileg gögn á skýran hátt þvert á margar platform generations án þess að viðmótið verði of flókið.









## Hugmynd 3 - Gagnvirkt Leikjasafn og Upplýsingabanki (Örugg & Raunhæf)  / Interactive Game Collection and Information Hub
### Notandi
Retro-leikjaaðdáendur og safnarar sem vilja skoða stórt safn leikja, rifja upp minningar og skoða upprunalegt media efni.

### Vandamál
Skipuleggur 13.603 leiki á einum stað og gerir þá auðveldlega aðgengilega án þess að notandinn fari villtur í gagnaflóðinu.

### Gögn sem hugmyndin notar
cover_image_path, box3d_path, screenshots, genre, platform_name, decade, developer, rating_stars_5

### Aðalflæði
1. Notandinn opnar myndrænt grid-yfirlit og síar samstundis eftir decade, platform eða genre (t.d. Platformer).
2. Notandinn smellir á leik og opnar ítarlega leikjasíðu með 3D box, screenshots, description og rating (rating_stars_5).
3. Notandinn smellir á heiti developer / publisher (t.d. SEGA eða Konami) á leikjasíðunni.
4. Kerfið birtir samstundis alla aðra leiki í safninu frá þeim developer / publisher.

### Af hverju gæti þetta verið gott verkefni?
Þetta er mjög skýrt, öruggt í framkvæmd og nýtir mikið af sjónrænum gögnum (3D box, kápumyndir, skjáskot) sem gerir lokaafurðina mjög glæsilega án þess að forritunin verði óyfirstíganleg.

### Helstu áhættur
Að tryggja að stóra myndræna grid-yfirlitið hlaðist hratt og síist mjúklega án seinkunar þegar unnið er með mörg þúsund leiki.








## Valin Hugmynd

Við veljum: Hugmynd 1 Tilmælavél og meðmælakerfi 

Ástæða: Okkur fannst báðum þessi hugmynd áhugaverð og mögulega nytsamleg.

Við erum að búa til tilmælavél og meðmælakerfi fyrir notendur sem hjálpar honum að leysa vandmálið í að leita að öðrum leik eftir að klára leik með því að slá inn leikinn sem þau kláruðu og fá tilmæli um leiki sem þeim gætu fundist skemmtilegir.

