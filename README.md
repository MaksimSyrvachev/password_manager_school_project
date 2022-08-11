# password_manager_school_project
My school project for python lessons, which represents simple password manager with using library for encoding and decoding whith help of unique key and also ability to store passwords in text file in encrypted form. Also README file will be written in Czech language, so you can translate.
# Úvod
Představme si, že máme hodně accountů (sociální sítě, media, maily atd.) v Internetu a chceme hesla od těchto accountů mít někde uložené v počítači. Ale nechceme zároveň aby se každý, kdo by se posadil za můj počítač mohl přečíst a využit tyto hesla (popřípadě můžeme chtít poslat hesla někomu jako soubor nebo packet). Z těchto bezpečnostních důvodu musíme mít soubor s těmi hesly zakódované a pro použití hesel musíme je nejprve dekódovat pomoci nějakého klíče, který budeme mít a umět s ním zacházet jenom my. Proto napsal jsem program, který kóduje a dekóduje hesla s využití vytvořeného námi klíče. V tomto README souboru popíšu základní princip fungování mého programu a přímo v programu popsal jsem každou funkci (její princip fungování), postup a logiku pomoci komentáře. 
# Co dělá můj program?
Rozhodl jsem realizovat svůj program pomocí OOP. Vytvořil jsem class My_pass_manager, do kterého jsem nejprve přidal konstruktér s proměnnými self.key (pro chování kliče), self.pass_dickt (pro chování webů a hesel k ním) a self.pass_web (pro chování jména souboru do ktérého se zapíše zakodováná hesla). Inicializoval jsem vše 3 hodnoty na prázdné (None). Pak jdou metody (funkce) tohoto classu, které jsem popsal pomocí komentáře v programu. Tím jsem vytvořil class, který může vytvořit a použit klič pro kódování hesel (a i čehokoliv), zacházet s už existujícím slovníkem hesel, zapisovat ho do souborů zakódovaná hesla, přidávat tam nová hesla k novým webům, nahrávat už zapsaná zakódovaná hesla z jakéhokoliv souboru v pracovní direktorii do programu v dekódovaném formátu při známém klíče pro další manipulace a určitě dostávat hesla k určitým webům. Pro manipulaci s tímto classem jsem vytvořil Menu, pomocí kterého můžeme volat funkcí vytvořeného objektu classa (person1). Např. pokud uživatel stiskne 1 (1. Create a new key), bude zavolána metoda objektu person1.create_key(). Realizace je provedená pomoci cyklusu while (switch v Python bohužel neexistuje). Pomoci toho Menu jsem realizoval interakce s uživatelem.
Program běží v terminalu.
# Závěr
Je to nekomplikovaný program, který určitě lze vylepšit, např. tím že přidáme metodu pro změnu hesla zapsaného do souboru webu atd. Ale tento program funguje a asi lze ho použit v reálném životě.
