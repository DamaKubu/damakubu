.. title: Disfunkcinės nuostatos ir laimingumas
.. slug: dns-and-happiness-survey-analysis
.. date: 2024-03-03 02:07:58 UTC+02:00
.. tags: 
.. category: 
.. link: 
.. description: Aprašau kažkiek analizę tyrimą kurį atlikau
.. type: text
.. has_math: true

.. class:: alert alert-info pull-left

.. contents::



.. sidebar:: TLDR:

   Hobininė psichologinės apklausos analizė. Tyriami teiginiai iš David D. burn knygos „Geros nuotaikos Vadovas“. Taip pat patvirtinama koreliacija tarp geros vaikystės ir religijos išlikimo. Tai yra vaikai sveikose šeimose perima tėvų verybes ir religiją. Gal vertingiau paklausyti mano `filmuko <https://youtu.be/_U70RkF1AHw>`_ apie šį tyrimą, jei norite suprast savo rezultatus 





Įvadas
========

Motyvacija, kam išvis tokį tyrimą atlikti?
-------------------------------------------

Moksliniai tyrimai naudoją mokslinę kalbą, o mano tyrime tokios kalbos atsisakyta.
Panašiai, kaip paleidus skruzdėle, eidami kiek kitokiu kelių rizikuojame atrasti kažką naujo, arba giliau patvirtinti esamus teiginius.


.. sidebar:: skruzdės principas

   Įsivaisduokime esame skrusdėlytė dirbanti kolonijai. Išorėje yra sudėtingas pasaulis mūms sunkiai suvokiamas, bet mūsų tikslas išsiaiškinti tą pasaulį. Verta eiti ten kur dar kitos skruzdės nebuvo, jeigu noriu, jog koloniją, sudarytų kuo geresnį aplinkos žemėlapį(modelį). Aišku realiame gyvenime, skruzdės ne žemėlapį sudarinėja, o ieško maisto, tad tik kartais gali sau leisti keliauti ir bandyti atrasti maisto šaltinius. Dažnai tenka sekti feromonais iki atrasto maisto šaltinio ir atgal į urvą. Tai manau labai puiki analogija mokslo progresui. Išties mėgsta mokslininkai vienas kitą sekti, bet gi būtent darydami dalykus kitaip, eidami į kitą pusę, galime atrasti kažką naujo.





Nesu psichologijos studentas, neturiu laiko skaityti psichologijos straipsnių, tad mano gauti rezultatai yra mažiau paveikti įprastų psichologus veikiančių sisteminių paklaidų. Kaip derinimasis prie esamų rezultatų, dogmų ar tradicijų.

Tad mano gautas rezultatas labiau nepriklausomas, nes nesiremiu, psichologinijos straipnsių masyvu, o daugiau būtent savo suvokimu ir patirtimi kuriant hipotezes. Tad esu ta skruzdė, kuri gal ir nieko nepeš, bet bent jau eina į kitą pusę. 

Matematinę statistikos dalį, manau atlieku geriau negu vidutinis psichologijos studentas. 

Ko pasekoje tyrimas išties unikalus, statistiškai tikslus ir itin nepriklausomas nuo įprastinių psichologų sisteminių paklaidų.




Disfunkcinių nuostatų skalė (DNS)
------------------------------------

DNS, tai David Burns, kognityvinės terapijos knygoje „Geros nuotaikos vadovas“ pristatyta apklausa, pagal kurią galima įsivertinti, savo daromas mąstymo klaidas, kurios gadina nuotaiką ir net vedą į depresiją. Taip pat knygoje pateikta ir depresijos apklausa, pagal kurią galima įsivertinti savo depresijos lygį.

Prieš du metus organiškai davus šias apklausas draugams radau esant koreliacijai tarp depresijos ir DNS. Visgi koreliacija buvo itin silpna, duomenys labai plačiai išsibarstę ir apklaustųjų skaičius išties mažytis 11 žmonių. 


.. figure:: /images/orginal_burns_vidurkis.png
   :width: 800
   :align: center
   
   Pirmasis tyrimas Burns depresija nuo DNS vidurkio, aiški neigiama koreliacija. Atrodo moterys raudoni taškeliai ir vyrai itin skiriasi.
   
:raw-html:`<br />`

 Nuo tada kirbėjo tyrimą kartoti su didesne imtimi ir su geresniais statistikos gabumais. Na esu čia 3 nakties, žiūrėkim kas gausis.


Depresijos skalę šiame tyrime pakeičiau į subjektyvaus laimingumo skale. Skruzdės principu, siekiant tvirto mokslo pravartu naudoti, kito autoriaus skalę ir kitokio tipo. Vietoj depresijos tiriame laimingumo lygį.

    Klausimai randomizuoti, tai yra neaišku apie kokį koncepta(pasitikėjima, meilę, anatomija,...) klausimas tiria.

    Taip pat pusę klausimų yra apversti, teigiamas atsakymas nebūtinai yra sveikas atsakymas. (Orginaliame teste teigiamas atsakymas visada buvo gerai. Tad žmogus, net neskaitydamas galėtų gauti labai aukštą rezultatą.)





Hipotezės( sugalvotos prieš renkant duomenis )
----------------------------------------------------------

Matematikas Aleksandras užsiminė, jog daugelis nežino kas per daiktas yra nulinė hipotezė. Man atrodo, daugelis nežino išvis kas hipotezė yra, nes pats iki trečio fizikos kurso maišiau ją su spėjimu.
Hipotezė, tai nėra spėjimas!
*Hipotezė* - falsifikuojamas pasaulio aiškinimas. *Falsifikuojamas* - eksperimentu galima parodyti, jog hipotezė neteisinga. Pagal, kai kuriuos mokslo filosofus hipotezę galima tik nuneigti, bet niekad jos negalime įrodyti.

*Nulinė Hipotezė* - jau specifiškas terminas, reiškiantis, „pradinį pasaulį nesant hipotezės deklaruojam efektui“, tai taškas nuo kurio atsispiriame tirdami savo hipotezę. 

Statistikoje, dažnas $H_0$ pavyzdys, tiriant dvi grupes:

$H_0$ - grupės yra paimtos iš tos pačios pradinės populiacijos

$H_1$ - grupės yra iš skirtingų populiacijų.

Bet jeigu randame, jog esant didelei imčiai grupės skiriasi, galime atmesti nulinę hipotezę, nes ji labai neįtikima.
Mėgstamas humanitarų p reikšmingumas nurodo tikėtinumą, jog rezultatas matomas galiojant $H_0$.


.. sidebar:: Permutacijų metodas(angl. permutation method)

   Rašydamas hipotezes nežinojau, jog mano sugalvotas algoritmas vadinasi permutacijų metodu ir plačiai naudojamas. Patikęs youtube videkas apie jį: `Videkas <https://www.youtube.com/watch?v=F8b_gxKPxG8&t=0s>`_ 

Kaip bebūtų prieš tyrimą sugalvojau tokias keturias hipotezes, dvi iš jų pasitvirtino, dvi silpnai. Spėkit kurios!

    1. Disfunkcinės nuostatos(DNS) lemia žmogaus nelaimingumą. Jei hipotezė teisinga, DNS ir laimės lygis turėtų stipriai koreliuoti.
    
    2. Iš anekdotinių savo pažįstamų, atrodo, jog žmonės keičia religija, jei turėjo disfunkcinę šeimą ir religijos nekeičia, jei turėjo sveiką ir gerą vaikystę. Koreliacijos nebuvimas tarp religingumo, bei šeimos disfunkcionalumo paneigtų hipotezę.
    
    3. Vyrai ir moterys stipriai skirasi: Šitą patestuoti galima atsitiktinai parinkti iš bendros krūvos parinkti dvi agentų grupes ir palyginti su moterų ir vyrų grupėmis. Hipotezė reiks atmesti, jei taikant permutacijų metodą nebus skirtumo tarp jų vidurkio.

    4. Moterys vidutiniškai turi aukštesnį emocinį intelektą, ko pasekoje turi mažiau disfunkcinių nuostatų. Bet dėl kitų priežasčių(pvz.: mėnesinių turėjimo), jų laimės indeksas nesiskiria nuo vyrų. Jei nematysime žymaus skirtumo tarp vyrų ir moterų laimės ir DNS koreliacijos tiesių, hipotezė bus paneigta.






Duomenų rinkimas
=================

Duomenis rinkau ~3 mėnesius, norėjau surinkti bent 100 surinkau ~40.
Naudojau psytoolkit [3]_ online apklausai vykdyti, specialiai pritaikyta psichologiniams tyrimams.
Patogu išimti duomenis. Bei yra minimalus interaktyvumas, pateikiau rezultatus tik atlikus testą.
Prižadėjau apklausoje, jog padarysiu analizę ir atsiųsiu rezultatus pasilyginant su kitais paštu.


.. sidebar:: proporcija

   Įdomu, jog monotoniškai auga moterų ir vyrų proporcija: 1.777 1.867 2.0 2.125.
    Moterų ne tik daugiau, bet jos ir ilgiau išlieka tyrimo eigoje.
   
**Kiek tiksliai žmonių dalyvavo tyrime?**

    * Tyrimo apklausa buvo atidarytas 180 kartų.
  
    * 18 vyrų ir 32 moterys atliko tyrimą dalinai arba pilnai. 
  
    * 15 vyrų ir 28 moterys atliko laimingumo testą ir atsakė į religijos klausimą. 
  
    * 12 vyrų ir 24 moterų atsakė į visus klausimus.
  
    * 8 vyrai ir 17 moterų įrašė savo el. paštą.




Analizė
===========

Jaučiuosi atlikęs itin išsamią analizę. Manau esmė galima iš esmės pateikti koreliacijos matrica.


Pirmiausia pateiksiu svarbiausius rezultatus


.. figure:: /images/koreliacija_matrica_1.png
   :width: 800
   :align: center
   
   Naudojamas Spearman koeficientas ir rodoma koreliacija tarp skirtingų konceptų. Pažymėtina būtent išankstinių hipotezių numatytos dvi koreliacijos yra didžiausios 0.51 ir 0.37. Pagal lentelę tokios koreliacijos reikšmės nurodo vidutinį koreliavimą.
   
   
.. figure:: /images/koreliacija_matrica_2.png
   :width: 800
   :align: center
   
   p reikšmingumas matrica(kuo mažesnė tuo geriau.)
   

Pateiksiu abu grafikus:


.. figure:: /images/DNS_vs_SHS.png
   :width: 800
   :align: center
   
   Disfunkcinės nuostatos versus laimingumo testo rezultatai. R, tai Pearsono koreliacija.
   


.. figure:: /images/religija_vs_vaikyste.png
   :width: 800
   :align: center
   
   Rezultatai, tarp vaikystės religijos keitimo ir pasitenkinimu vaikyste.


DNS
-----



.. figure:: /images/dns/koreliacijos_matrica_didelė.png
   :width: 800
   :align: center
   
   Spearmano koreliacinė matrica.
   
   
.. sidebar:: intervalas

   Standartinis nuokrypis, standartinė paklaida ir patikimumo intervalas yra susiję, bet atskiri dalykai `blog post <https://www.data-to-viz.com/caveat/error_bar.html>`_. Standartinė paklaida, tai standartinis nuokrypis padalintas iš grupės skaičiaus šaknies. O patikimumo intervalas, tai standartinė paklaida padauginta iš stjudento koeficiento atitinkam imties skaičiui.

.. figure:: /images/dns/DNS_voras.png
   :width: 800
   :align: center
   
   Skritulinė vidurkio histogramą, nurodyti standartinės paklaidos intervalai.



Moterys vs. vyrai
------------------



.. sidebar:: Nulinė hipotezė

   $H_0$ - moterų ir vyrų DNS nesiskiria.


Pagal hipotezę vyrų ir moterų DNS turėtų būti aukštesnis, nes moterų vidutinis emocinis intelektas aukštesnis.


Išties moterų dns vidutinis suminis DNS aukštesnis dviem balais, bet naudojant permutacijų metodą, matome, jog rezultatas tikėtinas ir esant nulinei hipotezei.

.. figure:: /images/dns/moterys_vs_vyrai.png
   :width: 800
   :align: center
   
   Rodykle rarodome vyrų vidurkio ir moterų skirtumą. O histograma gaunama naudojant permutacijų metodą: sudedam abi grupes į vieną masyvą, tada iš masyvo traukiam dvi grupes ir jas lyginame, daug lyginimo rezultato reikšmių ir sudaro histogramą. Matome, jog gauta vertė išties tikėtina esant $H_0$.


Bet atskiriem DNS kategorijai pripažinimas išties yra reikšmingas vidurkių skirtumas tarp vyrų ir moterų:

.. figure:: /images/dns/pasiekimai.png
   :width: 800
   :align: center
   
   Moterys pasiekimų atžvilgiu turi sveikesnį nusistatymą. Reikšmingumas $p = 0.084$.


.. figure:: /images/dns/pripažinimas.png
   :width: 800
   :align: center
   
   Iš pirmo žvilgsnio atrodo, jog panaši sitauacija ir su pasiekimais: moterys pasiekimų atžvilgiu turi sveikesnį nusistatymą Bet atkreipus dėmesį rodyklėlės vietą, itin tikėtina, jog atsitiktinai jinai ten atsidurė $p = 0.64$.


.. figure:: /images/dns/meilė.png
   :width: 800
   :align: center
   
   Matome, jog vyrų ir moterų grupės meilės aspektu statistiškai nesiskiria. Analogiškai nesiskiria ir  perfekcionizmas, bei galia.

.. figure:: /images/dns/atlygiolaukimas.png
   :width: 800
   :align: center
   
   Atrodo yra neigiamas skirtumas, bet vėlgi reikšmingumas $p = 0.7$, tai išvadų daryti negalim.



Dėl pilnumo galime pažiūrėti, kaip skirasi vyrų ir moterų atsakymai



.. figure:: /images/dns/vyrai_vs_moteris_religija.png
   :width: 800
   :align: center
   
   Štai lyginame moteris ir vyrus religijos, bei vaikystės klausimu.


Ahm norint tirti vyrų ir moterų skirtumus reikia didesnės imties, manau tik parodo,jog esame visai panašūs. Nors turiu mintį, kad savanoriškai apklausą atlieką „moteriškesni“ vyrai, tai vėlgi sisteminė paklaida dėl neatsitiktinės imties tikrai yra.


:raw-html:`<br />`





Išvados
----------

    * DNS ir subjektyvus laimingumas išties koreliuoja $R = 0.59$ ir $p = 0.00014$.
    
    * Religijos keitimas ir vaikystės pasitenkinimas koreliuoja $R = 0.33$ ir $p = 0.033$
    
    * Moterų ir vyrų DNS rezultatai skiriasi labai silpnai.




Šaltiniai:
-----------

.. [1]  Lyubomirsky, S. & Lepper, H. S. (1999). A measure of subjective happines: Preliminary reliability and construct validation. Social indicators research, 46, 137-155.


.. [2] Stoet, G. (2010). PsyToolkit - A software package for programming psychological experiments using Linux. Behavior Research Methods, 42(4), 1096-1104. Stoet, G. (2017). PsyToolkit: A novel web-based method for running online questionnaires and reaction-time experiments. Teaching of Psychology, 44(1), 24-31.

.. [3] Mano Youtube filmukas apie šį tyrimą: `filmukas <https://youtu.be/_U70RkF1AHw>`_ 

.. [4] github atviri tyrimo duomenys: `Github <https://github.com/DamaKubu/Depresija_ir_Nuostatos>`_ 

.. [5] Bei google collabas, kur galima pažaist su duomenimis nieko neinstaliuojant.
    `tyrimo collabas <https://colab.research.google.com/drive/1Y70bVFKRjhydVF1sFl_ZOQ4QwlZDURDO?usp=sharing>`_




