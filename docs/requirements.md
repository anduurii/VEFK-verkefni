# Requirements



## Tilgangur
Við erum að búa til tilmælavél og meðmælakerfi fyrir notendur sem hjálpar honum að leysa vandmálið í að leita að öðrum leik eftir að klára leik með því að slá inn leikinn sem þau kláruðu og fá tilmæli um leiki sem þeim gætu fundist skemmtilegir.


## Aðalnotandi
Leikjaspilarar sem eru búnir að klára leik sem þeim þótti frábær og vilja finna næsta leik til að spila án þess að eyða mörgum klukkustundum í að leita.


## Vandamál
Leysir valkvíða / choice paralysis. Í stað þess að leita í gegnum 13.000+ leiki, fær notandinn ábendingar byggðar á tölfræðilegum líkindum og rating.


## Out of scope
Notandinn reynir að útskýra leikinn sem hann vill fá meðmæli um sem passar best.


## Functional requirements
FR-01: Notandinn getur sláið inn nafn á leik og fengið 5 líkustu leikirnar í gagnagrunninum. (Sjá NFR-03)
FR-02: Notandinn getur smellið á meðmælin til að skoða screenshots, description og rating.
FR-03: Notandi skrifir titillinn og kema upp líkustu titlarnir til þess að notandi þarf ekki að skrifa fullkomlega.
FR-04: Notandi getur valið að fá fleiri tilmæli sem eru ekki eins lík og upprunalegi leikurinn.
FR-05: Notandi getur búið til account og merkt við leikir sem hann hefur klárað.

## Non-functional requirements
NFR-01: Kerfi getur lesið og unnið með gögnunum í gagnagrunninum.
NFR-02: Kerfi getur birt basic profile fyrir leik út frá gögnum í gagnagrunninum.
NFR-03: Kerfi getur greint og reiknað líkustu leikirnar í gagnagrunninum út frá genre, developer, decade og rating.
NFR-04: Kerfi getur geymt upplýsingar um notendur á öruggan hátt og síað tilmæli frá hvaða leiki notandi hefur klárað.
NFR-05: x

## User stories
US-01: Sem Leikjaspilari vil ég fá tilmæli um góða leiki svo að ég þurfi ekki að leita sjálfur.
US-02: Sem Leikjaspilari vil ég skoða frekari upplýsingar um tilmælin svo að ég geti verið viss um að þetta sé góð tilmæli.
US-03: Sem Leikjaspilari vil ég geta fengið ólíkar tilmæli svo að ég fæ leiki sem eru aðeins öðruvísi en það sem ég spil venjulega.
US-04: Sem Leikjaspilari vil ég getað búið til account og skráð leiki sem ég hef klárað svo að ég fæ ekki leiki sem ég er búinn með.

## Open questions

Hvernig á að vega gögnin til þess að finna líka leikir.