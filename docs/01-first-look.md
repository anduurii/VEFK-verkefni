# Fyrsta skoðun á gagnasafninu



## Hópur

    Nöfn: 
    Karl Andri Manloloyo
    Hringur Hrafnkelsson


## Gagnaskrár sem við skoðuðum

    DATA_DICTONARY.md
    games_master_dataset.csv
    consoles_platforms_dataset.csv
    games_master_dataset.csv
    genres_and_tags_summary.csv
    developers_and_publishers.csv


## Stærð gagnasafnsins

    Fjöldi leikjafærslna: 36140
    Fjöldi dálka: 38
    Fjöldi platforma: 14

## 10 athuganir um gögnin

    1. 887 duplicate game_id
    2. 513 unknown developers
    3. 20% af leikjunum vantar rating
    4. stundum rom_size_mb = 0
    5. players_raw er frjáls texti
    6. Sega er með mest leikir = 786 leikir. 251 meiri en Konami sem er næst mest.
    7. u.þ.b. 42% developers eru bara með 1 leik.
    8. Top 6 genre eru 68% af leikjunum. Neðstu 5 genre eru 15%.
    9. Útgáfu dagsetning vantar eða ónákvæm hjá mörgum leikjum.
    10. u.þ.b. 3000 af leikjunum eru arcade.

## 5 spurningar sem við viljum rannsaka

    1. Eru leikirnar með það sama game_id líkir?
    2. Hvaða game_id kemur fram oftast?
    3. Hvað meðalrating af öllum genres?
    4. 
    5.

## 3 atriði sem komu okkur á óvart

    1. 887 duplicate game_id
    2. 513 unknown developers
    3. Sega er með mest leikir = 786 leikir. 251 meiri en Konami sem er næst mest.




## 5 atriði í gögnunum sem gætu skapað möguleika fyrir vefkerfi

    PC Builder / Vélbúnaðarreiknir: Ákvarðar hvers konar tölva eða vélbúnaður vantar til að geta spilað eða hermt leikina sem þú vilt spila.

    Wikipedia / Lýsingar fyrir leikjunum: Upplýsingabankamót með sögu leikjanna, myndum, skjáskotum og lýsingum.

    Leikjasafn: Miðlægt svæði til að fletta í gegnum og sía allt leikjasafnið eftir flokkum, útgáfuárum og tölvukynslóðum.

    Leitarkerfi fyrir fjölspilun og samkvæmisleiki: Sía sem finnur leiki sérstaklega út frá fjölda spilara (t.d. fyrir 2-4 spilara á sama skjá).

    Tilmælavél / Ráðleggingarkerfi: Ráðleggur notendum svipaða eða falda gæðaleiki út frá uppáhaldsleikjum þeirra, einkunnum og flokkum.




## Mögulega notendur

    Retro-aðdáendur og safnarar: Nota Leikjasafnið og Wikipedia-lýsingarnar til að kanna sögu leikjanna, fletta upp upplýsingum og skoða kápumyndir.

    Tæknisinnar og herma-notendur: Nota PC Builder / Vélbúnaðarreikninn til að finna réttan vélbúnað og herma fyrir ákveðnar leikjatölvur.

    Vinahópar (Spilakvöld): Nota Fjölspilunarleitarvélina til að finna leiki sem styðja 2–4 spilara á sama skjá.

    Leikjanámsfúsir spilarar: Nota Tilmælavélina til að finna falda gæðaleiki út frá einkunnum og uppáhaldsflokkum.

    Aðdáendur leikjaframleiðenda og sögunörðar: Nota kerfið til að skoða sögu og tölfræði ákveðinna útgefenda og þróunaraðila (t.d. SEGA eða Konami) í gegnum áratugina.





## Hugmynd 1 - gagnleg fyrir ákveðinn notanda

    Hugmynd 1 á að leysa skýrt vandamál fyrir ákveðinn notanda

    -----------------------------------------------------------------

    Tilmælavél og meðmælakerfi    /   Recommendation Engine and Recommendation System

    Hver notar kerfið? 
        Leikjaspilarar sem eru búnir að klára leik sem þeim þótti frábær og vilja finna næsta leik til að spila án þess að eyða mörgum klukkustundum í að leita.

    Hvaða vandamál leysir það? 
        Leysir valkvíða / choice paralysis. Í stað þess að leita í gegnum 13.000+ leiki, fær notandinn persónusniðnar ábendingar byggðar á tölfræðilegum líkindum og rating.

    Hvaða raunverulegu gögn úr gagnasafninu notar það? 
        Genre, Rating, Developer, Images

    Hvað gerir notandinn skref fyrir skref? 
        Notandinn slær inn eða velur leik sem hann heldur upp á (t.d. Castlevania: Symphony of the Night).
        Kerfið greinir einkenni leiksins (genre, developer, decade).
        Tilmælavélin reiknar út og birtir topp 5 leiki sem líkjast valda leiknum og hafa háa rating (rating_score_pct).
        Notandinn getur smellið á meðmælin til að skoða screenshots, description og rating.

    Hvað gæti verið erfitt?
        Að hanna einkunnagjafar- og líkindaalgoritmann þannig að hann mæli með réttum leikjum (t.d. að vega saman genre_detailed og rating_score_pct á réttan hátt).



## Hugmynd 2 - skapandi eða óvenjuleg

    Hugmynd 2 á að nota gögnin á áhugaverðan hátt. Hún má vera djarfari en hugmynd 1.

    -----------------------------------------------------------------------

    Retro Time Machine & Console Wars

    Hver notar kerfið?
        Leikjasögunörðar og nostalgíuleitendur sem vilja kanna ólík tímabil tölvuleikjasögunnar eða bera saman samkeppnisaðila á leikjamarkaðnum.

    Hvaða vandamál leysir það?
        Gerir söguleg tölvuleikjagögn lifandi og sjónræn í stað flatrar leitar. Leysir skort á uppgötvun á óþekktum leikjum með því að breyta leit í gagnvirkt tímaferðalag og random discovery.

    Hvaða raunverulegu gögn úr gagnasafninu notar það?
        Platform Generation, Decade, ROM Size, Developer, 3D Box, Screenshots

    Hvað gerir notandinn skref fyrir skref?
        Notandinn velur tímabil eða console wars (t.d. 16-bita tímabilið: SEGA Genesis vs. Super Nintendo).
        Kerfið birtir gagnvirka tímalínu og samanburð á skráarstærðum leikja (rom_size_mb), rating og yfirburðum developer / publisher.
        Notandinn ýtir á „Time Warp / Slot Machine“ hnappinn til að fá random discovery.
        Kerfið dregur fram faldan gæðaleik frá því tímabili ásamt 3D box (box3d_path), screenshots og developer sögu.

    Hvað gæti verið erfitt?
        Að hanna myndræna tímalínu og taka saman tölfræðileg gögn á skýran hátt þvert á margar platform generations.


## Hugmynd 3 - raunhæf og örugg

    Hugmynd 3 á að vera eitthvað sem hópurinn telur mjög líklegt að hægt sé að klára vel. Hún má vera einfaldari, en
    þarf samt að vera meira en bara listi og search.

    Hún þarf að hafa skýran notanda og að minnsta kosti eitt raunverulegt notendaflæði.

    ---------------------------------------------------------------------

    Gagnvirkt Leikjasafn og Upplýsingabanki      /    Interactive Game Collection and Information Hub 

    Hver notar kerfið?
        Retro-leikjaaðdáendur og safnarar sem vilja skoða stórt safn leikja, rifja upp minningar og skoða upprunalegt media efni.

    Hvaða vandamál leysir það?
        Skipuleggur 13.603 leiki á einum stað og gerir þá auðveldlega aðgengilega án þess að notandinn fari villtur í gagnaflóðinu.

    Hvaða raunverulegu gögn úr gagnasafninu notar það?
        Cover Images, 3D Box, Screenshots, Genre, Platform, Decade, Developer, Rating

    Hvað gerir notandinn skref fyrir skref?
        Notandinn opnar myndrænt grid-yfirlit og síar samstundis eftir decade, platform eða genre (t.d. Platformer).
        Notandinn smellir á leik og opnar ítarlega leikjasíðu með 3D box, screenshots, description og rating (rating_stars_5).
        Notandinn smellir á heiti developer / publisher (t.d. SEGA eða Konami) á leikjasíðunni.
        Kerfið birtir samstundis alla aðra leiki í safninu frá þeim developer / publisher.

    Hvað gæti verið erfitt?
        Að tryggja að stóra myndræna grid-yfirlitið hlaðist hratt og síist mjúklega án seinkunar.