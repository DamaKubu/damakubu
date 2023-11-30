.. title: Genų dreifas
.. slug: genų dreifas
.. date: 2023-11-25 22:04:07 UTC+02:00
.. tags: Evoliucija, DI
.. category: 
.. link: 
.. description: Kelios mintys apie vieną iš pagrindinių evoliucinių mechanizmų genų dreifą.
.. type: text
.. has_math: true

.. class:: alert alert-info pull-left

.. contents::



.. sidebar:: TLDR:

   *Genų dreifas* - vienas iš pagrindinių evoliucijos mechanizmų. Atsiranda dėl atsitiktinumo, ryškiausiai pasireiškia mažose populiacijose, mažina genetinę įvairovę. Dėl jo populiacijoje įsitvirtina aleliai nebūtinai turintys adaptacinę naudą, gali būti net žalingi.


Šiuo metu turiu bio-evoliucijos kursą jame užtikau vieną smagų konceptuką - *genų dreifas*, ko pasekoje kardinaliai pasikeitė mano požiūris į evoliuciją.


Evoliucijos Mechanizmai
=========================

Darvino *naturali atranka* yra vienintelis evoliucinis mechanizmas pastoviai keliantis organizmų adaptyvumą(fitness) [1]_. Didesnę tikimybę turi išgyventi tie kurie geriau prisitaikę prie aplinkos, per daug kartų individų prisitaikymas didėja.  Ji aplikuojama, kai

    1. variacija

    2. paveldimumas

    3. adaptyvumas reikšmingas

Bet yra daugelis kitų mechanizmų, kodėl genai išplinta populiacijoje.

Genų tranzavimas
-------------------

Genas A esantis fiziškai arti geno adaptyvumą keliančio geno B, tranzuoja per jį į populiaciją. Pvz.: Karvėse genas A atsakingas už daugiau pieno, o genas B už mažesnį vaisingumą. Dirbtinė žmonių atranka populiacijoje įtvirtiną A geną, bet su juo keliauja ir genas B mažinantis karvių vaisingumą [2]_.

:raw-html:`<br />`

Partnerio pasirinkimas
-------------------------

Vienos lyties sisteminis kažkokių savybių kitoje lytyje preferavimas veikia kaip atranka. Gamtoje įprastai, tai labiau daro viena lytis ir dažniausiai tai būna patelės, dėl ko dažnai patinėliai atrodo įspudingiau.
(Įdomu, jog patelių preferuojamos savybęs nebūtinai didina patinėlių prisitaikomumą prie aplinkos).


.. sidebar:: 

    „Kai stebiu povo uodega mane supykina.“
    - 1860m. Darvinas [3]_

.. figure:: /images/Peacock.jpg
    :width: 800
    :align: center
    :alt:  nuotrauka
    
    Povas bandantis suvilioti patelę. 




Genų dreifas
---------------

.. sidebar:: Martingalis ir Markovo procesas

    Puria urnos pavyzdys matematiškai yra *martingalis*, kuris apibrėžiamas taip:

    - Martingalio vertė baigtinė esant baigtiniam laikui: :math:`\forall n, X_n < \infty`

    - Martingalio tikėtiniausia vertė yra paskutinė stebėta vertė: :math:`\mathbb{E}[X_{n+1}|\{X_n, ..., X_{0}\}] = X_n`

    Taip pat jis yra Markovo grandinė, nes neturi jokios atminties. 
    
    
Dėl imties paklaidos kylantis atsitiktinio geno įsitvirtinimas populiacijoje. 

.. figure:: /images/genudreifas.png
   :width: 800
   :align: center
   
|   **Pavyzdys**: 
|   paimkime maišelį su 50 baltų ir 50 juodų rutuliukų. 
|   Iš maišelio paimkime 10 rutuliukų tikėtina baltų ir juodų skaičius skirsis tarkim 3 ir 7. 
|   Tada šia imties proporcija užpildykim naują maišiuką su 30 ir 70.
|   Vėl imkime 10 rutuliukų ir ištraukiam visus 10 juodų.
|   Betkokia nauja imtis visada duos juodus.
|   Tai yra rutuliukų populiacijoje įsitvirtino juodieji, nors neturi jokio adaptacinio pranašumo. 










:raw-html:`<br />`

Žaidimai ir klaidinanti intuicija.
=======================================

.. sidebar:: Aleliai
   
   Dėl chromosomų organizmai turi dvi versijas to paties geno - *alelius*.
   
   Kurią versija naudos organizmas priklausys nuo paties alelio, jei alelis *dominuojantis* tai jis ir pasireišks.
   Pavyzdžiui ruda akių spalvą koduoja dominuojantis alelis R, todėl rudakiai tėvai Rm gali turėti mėlynakius vaikus: 
   
   (Rm + Rm) -> (RR Rm mR mm).
   
   Mėlynakis bus tik mm, kiti vaikai (RR Rm mR) rudakiai.
   Mėlynos spalvos alelis m - *recesyvus* [4]_ - pasireiškia, tik tada kai nėra dominuojančio.
   
   Beje mėlynakiai tėvai negali turėti rudakio vaiko:
   
   (mm + mm) -> (mm mm mm mm)
   
Įdomu, jog tikimybė, kad ilgainiui alelis įsitvirtins populiacijoje yra lygiai pradinis alelio dažnis populiacijoje. [#moran]_ Tai yra jei 10% žmonių turi alelį A, tikimybė, jog jis įsitvirtins populiacijoje yra lygiai 10%.
Man tai neintuityvu, *kodėl*? Tarkim imame imtį iš maišelio ir ištraukiam daugiau juodų rutuliukų. Pagal imties proporcija pripildom maišelį ir traukiam naują imtį, tikimybė jog ištrauksiu juodus rutuliukus tik padidėja. Tai yra procesas turėtų turėti kažkokį tai polinkį. Pabandysiu intuiciją patikrinti modeliuku:

    Metu nesimetrinę monetą iškristi herbui tikimybė p, o iškristi monetai tikimybė 1-p, kur p lygi alelių dažniui populiacijoje. Jeigu krenta herbas pakeliu alelių skaičių populiacijoje +1, jeigu moneta sumažinu -1.


Galima įsivaisduot, jog individas miršta, o jo vieta užpildo kito atsitiktinai išrinkto individo kopja.



.. code-block:: python
            
            N = 100    #populiacija
            b = 25     #pradinis alelių skaičius populiacijoje
            
            random = np.random.uniform(0,1,MAX_LENGTH)  
            
            for w in random:
                if b == N or b == 0: 
                    break
                   
                elif w < b/N: 
                    b+=1      #pasirenka šitą su tikimybe  b/N
                else:        
                    b-=1      #pasirenka šitą su tikimybe 1 - b/N




.. figure:: /images/manomodelis1.png
   :width: 800
   :align: center
   
   Matome, jog veikia kažkokia stuma išstumianti alelį į kraštą( suteikianti atsitiktiniam jūdėjimui eksponentės pavidalą).

.. figure:: /images/sigmoide.png
   :width: 800
   :align: center
   
   X ašyje pradinis alelio dažnis populiacijoje b, o y ašyje tikimybė, jog jis įsitvirtinis populiacijoje. 
   Pradžioje alelį turi pusė populiacijos.  
   Gavau gražią sigmoidę, bet teiginys nepasitvirtino! Gi tikėjomės gražios tiesės!

Purya(maišelių modelis):
----------------------------------
Pabandykime implementuoti jau minėta maišelių pavyzdį: 

.. code-block:: python

     # maišelių algoritmas
     
     for _ in range(MAX_LENGTH):
        
        # paimu 200 agentų imtį iš populiacijos masyvo
        
        imtis = np.random.choice(populiacija, 200) 
        
        #  padarau visą populiacija su imties proporcija
        
        Juodi = int(N / 200) * imtis.sum()  
        populiacija = np.concatenate((
                      np.ones(Juodi, dtype=np.int8),
                   np.zeros(N-Juodi, dtype=np.int8)))

.. figure:: /images/purya.png
   :width: 800
   :align: center
   
   Pradžioje alelį turi pusė populiacijos. 
       

    
.. figure:: /images/purya2.png
   :width: 800
   :align: center
   
   Pradžioje alelį turi 25% populiacijos. 




.. figure:: /images/purya3.png
   :width: 800
   :align: center
   
   Na, o paleidus maišelių algoritmą su įvariais pradiniais alelių kiekiais populiacijoje ir skaičiuojant, kiek alelių įsitvirtino, o kiek išnyko, išties gauname gražią tiesę. Neveikiant kitiems evoliuciniams mechanizmas, jei pradinėje populiacijoje 10% narių turėjo garbanių geną, tai tikimybė, jog praėjus pakankamai laikui visi turės garbanių geną yra 10%. 
   

    
Kodėl intuityvus modelis neteisingas?
-------------------------------------

    1. **Hipotezė** pagal pirmąjį modelį miršta nebetkoks individas, o **neturintis alelio** tada jį pakeičia turintis arba neturintis. Tad vyksta sistemingas mažinanimas individų neturinčių alelio, tai ir būtų ta pirmame grafike stebėta nepaiškinta *stuma* suteikianti atsitiktiniam judėjimui eksponentiškės formą.

        - Bet tada pirmas grafikas turėtų būti nesimetrinis, t.y. lenktis labiau į vieną pusę. Visgi judėjimai atrodo simetriniai. 

Visgi pabandykim pamodifikuoti pradinį modelį, kas jei įdėsime papildomą atsitiktinumą renkantis mirštantį individą:

.. code-block:: python
            
            N = 42**2    #populiacija
            b = N/2      #pradinis alelių skaičius populiacijoje
            
            random  = np.random.uniform(0,1,MAX_LENGTH)  
            random2 = np.random.uniform(0,1,MAX_LENGTH)  
            
            for w in zip(random, random2):
            
                if b == N or b == 0: 
                    break
                   
                elif w < b/N:
                    if w2> b/N:
                        b+=1
                        
                else:
                    if w2 < b/N:
                        b-=1


.. figure:: /images/modifikuotas1.png
   :width: 800
   :align: center
   
   Rezultatas primena literatūroje pateiktą. Bet kodėl?
   
:raw-html:`<br />`



Kodėl modifikuotas modelis yra lygiavertus imties ėmimui
---------------------------------------------------------


.. figure:: /images/fuckthis.png
   :width: 800
   :align: center
   
|   Paaiškinimas: $w, w_2$ yra atsitiktiniai skaičiukai iš to paties simetrinio skirstinio, o $P = b/N$ dažnis. 


:raw-html:`<br />`


Metam nesimetrinę monetą ir renkamės juodą arba baltą rutuliuką, pasirinkta rutuliuką pakeičiam dar kartą mesdami nesimetrinę monetą juodu($p$) arba baltu($1-p$) rutuliuku. Nors tikimybės pasirinkti juoda ar baltą rutuliuką skiriasi, bet kadangi yra du lygūs metimai, jie vienas kitą išbalansuoja.

|  Padidinti populiacija vienu juodu rutuliuku:
|  pirmiausia turime ištraukti baltą $p$, o po to ištraukti juodą $1-p$.

|  Sumažinti populiacija vienu juodu rutuliuku:
|  pirmiausia turime ištraukti juodą $p-1$, o po to ištraukti juodą $p$.


:raw-html:`<br />`


Matematiškai, kadangi $w$ lygiavertis $w_2$, tai tikimybė būti didesniem ar mažesniem už p lygiai tokia pati.

.. math::

    \mathbb{P}[w_2>p] = \mathbb{P}[w>p]
    
    \mathbb{P}[w_2<p] = \mathbb{P}[w<p]
    
    


Tada tikimybė padidinti populiacija vienu baltu :math:`\mathbb{P}[b++]` arba vienu juodu rutuliuku yra lygi:
   
.. math::
    \mathbb{P}[b++] = \mathbb{P}[w>p]\mathbb{P}[w_2<p] = \mathbb{P}[w_2>p]\mathbb{P}[w<p] = \mathbb{P}[b--]
   

Kuo didesnė populiacija, tuo genų dreifo reiškinys yra lėtesnis
---------------------------------------------------------------

Kviečiu pačius pabandyti patikrintį sekanti genų dreifo teiginį:
Tikėtiniausias laikas reikalingas įsitvirtinti aleliui tiesiogiai proporcingas populiacijos dydžiui: :math:`\mathbb{E}[T] \propto N`.


.. figure:: /images/genudreifas2.png
   :width: 700
   :align: center

   Šaltinis vikipedija: https://en.wikipedia.org/wiki/Genetic_drift





Apibendrinta Evoliucija
-----------------------

.. sidebar:: Genų pernešimas
    
    Dabartinis didėjantis globalumas tikėtina ateina iš lengvesnės informacijos perdavimo(lengvo keliavimo) biologiškai šis mechanizmas vadinamas "genų pernešimo"(tarp izoliuotų populiacijų, individai perneša kultūrines idėjas), kas automatiškai homogenina pasaulio kultūrą.




:raw-html:`<br />`

Taikant apibendrintą evoliuciją galima iškart naudotis genų dreifo sąvoka,
atsakant ir į nebiologinius klausimus tokius kaip - „kodėl dauguma europiečių krikščionys?“

    Genų dreifo neužtenka [#zaratrusta]_, darant prielaida, jog žmonės gyvena apie 40 metų ir savo religijos nekeičia. Praėjo vos :math:`\approx 50` kartų nuo jėzaus gimimo, o agentų skaičius milijono eilės. Tad genų dreifas kaip vienintelis apibendrintos evoliucijos veiksnys nebūtų spėjęs taip stipriai suvienodinti europiečių. 



Pabaigai
========

Siūlau patiems išbandyti tyrimu pagrįstą simuliacija [#edu]_ https://cartwrig.ht/apps/genie/ kuri padės perprasti genų driftą.

Simuliacijos ir chaoso kodas, bei BUS užrašai: https://github.com/DamaKubu/bioevoliucija/




Šaltiniai:
-----------

.. [1] https://www.nature.com/scitable/knowledge/library/natural-selection-genetic-drift-and-gene-flow-15186648/?ref=scienceandpandas.com

    Anglų kalba trumpas skaitinėlis ta pačia tema, šiek tiek iš kitos pusės ir detaliau.

.. [2] Iš bio-evoliucijos BUS'o paskaitos.

.. [3] https://www.phaidon.com/agenda/photography/articles/2016/november/16/why-darwin-was-confused-by-birds/

.. [4] https://knowyourdna.com/are-blue-eyes-recessive/

.. [#edu] Genie: an interactive real-time simulation for teaching genetic drift
   https://evolution-outreach.biomedcentral.com/articles/10.1186/s12052-022-00161-7
   
.. [#moran] https://services.math.duke.edu/~rtd/cmodels/Moran.pdf

.. [#zaratrusta] Draugas Zaratrusta į šitą atkreipė dėmesį, dėkui.


