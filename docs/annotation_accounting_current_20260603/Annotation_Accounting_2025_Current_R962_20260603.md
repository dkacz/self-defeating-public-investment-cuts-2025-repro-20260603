# Rozliczenie anotacji po pełnej refinacji 2025

Data: 2026-06-03

Ten dokument rozlicza dwie grupy uwag merytorycznych. Pierwsza to cztery nowe anotacje R953 dodane do poprzedniego rozliczenia. Druga to uwagi domknięte wcześniej zbyt płytko, które mapa otwartych uwag wskazała jako wymagające pogłębienia. Każdy wpis pokazuje, co operator podkreślił, co było słabe wcześniej, jak praca to zaadresowała oraz dosłowny fragment obecnego manuskryptu, który tego dowodzi.

Status dokumentu: zamknięty po pełnym audycie Pro. GPT Pro 5.5 w piątej rundzie zwrócił werdykt 10/10 dla manuskryptu i 10/10 dla notebooka, bez wymaganych poprawek. Każdy cytat poniżej jest dosłowny z żywego manuskryptu i został niezależnie zweryfikowany pod kątem obecności i głębokości. To jest istotna różnica wobec poprzedniej wersji, która niosła etykiety "Status przed Pro" i jeden źle dopasowany cytat. Patrz sekcja procesowa na końcu.

## Wpływ na paper i notebook

Paper został zmieniony merytorycznie w sekcji 1.1, czyli w opisie bazy Komisji, oraz w sekcji 1.2, czyli w krytyce literatury (Borys, Ciżkowicz, Rzońca oraz Alesina i pokrewni). Poprawiono też dwie pozycje bibliograficzne. Notebook nie zmienił żadnej liczby, a jego warstwa czytelności została przepisana i ponownie wykonana, z zachowaniem bajtowo identycznego kodu.

Chronione liczby pozostają nietknięte: 55.1, 106.8, 2.87, 2.37-2.91, 2.59, 2.23, 1.78, 1.94, salda -10 i -3.9, próg 60, marginesy długu 2036 (7.7, 7.3, 4.3, 3.7), zakres 1.7-3.5 oraz p-wartości 0.002, 0.003, 0.080, 0.461. Pro potwierdził ich obecność i odtwarzalność z dostarczonych plików wynikowych.

# Klaster A: baza Komisji, arytmetyka zamiast instytucji

## A1 (N01, R953-G1, M05): nierealizm bazy ma być arytmetyczny, nie głównie instytucjonalny

**Podkreślenie operatora:** ekonomiczny i instytucjonalny sens bazy Komisji.

**Anotacja operatora:** perspektywa jest za mało post-keynesowska, lepiej nacisk na nierealistyczność założeń modelu Komisji, a nie głównie na to, że aktorzy nie reagują.

**Co było słabe wcześniej:** wcześniejsze zamknięcie opierało nierealizm głównie na argumencie instytucjonalno-behawioralnym, że rynki, instytucje i politycy mieliby nie reagować na narastający dług.

**Obecny fragment paperu:**

> The implausibility is arithmetic before it is behavioural, and it can be read directly off the Commission's own inputs. The baseline's implied nominal interest rate on government debt rises from about 4.8 percent in 2025 to about 6.2 percent in 2036, and the implied real rate rises from roughly 1.2 percent to roughly 3.4 percent over the same span. The interest-growth differential, favourable in the early years, changes sign in the course of the projection: nominal growth exceeds the implied interest rate until 2029 but falls short of it from 2030 onward, so the snowball term that initially lowers the ratio turns into one that raises it. By 2036 the differential alone adds about 0.9 percentage point to the debt ratio each year before any primary deficit is counted. Evaluating that condition at the 2036 debt ratio of 106.8 percent of GDP and the baseline's own 2036 differential, stabilising the ratio would require a primary surplus of about one percent of GDP, whereas the baseline assumes a primary deficit near -3.9 percent. The distance between the assumed balance and the debt-stabilising balance is therefore close to five percentage points of GDP.

**Dlaczego uznajemy to za zaadresowane głęboko:** ciężar argumentu przeniesiono na arytmetykę długu. Implikowana ścieżka stopy nominalnej i realnej, zmiana znaku różnicy stopa-wzrost w 2030, efekt kuli śnieżnej około 0.9 punktu rocznie oraz luka około pięciu punktów PKB między saldem założonym a stabilizującym są policzone wprost z wejść Komisji. Zdanie o braku reakcji aktorów zostało zdegradowane do "points the same way", a reguły krajowe do roli tła.

**Widoczne dowody i źródła:** warunek stabilizacji długu z ECB WP2486 (Checherita-Westphal i Domingues Semeano, 2020), zoperacjonalizowany na wejściach DSM2025 Komisji. Niezależne przeliczenie w `proposals/commission_baseline_arithmetic.md`.

**Walidacja Pro:** wymiar A (arytmetyka) PASS. Pro niezależnie odtworzył człon kuli śnieżnej 0.9060 punktu, saldo stabilizujące 0.9487 procent oraz lukę 4.8423 punktu.

**Ograniczenie:** to jest korekta interpretacji bazy Komisji, bez nowej estymacji.

**Status:** zamknięte po Pro 10/10.

## A2 (F02): ciężar z reguł krajowych przeniesiony na argument arytmetyczny

**Podkreślenie operatora:** nacisk na krajowe reguły fiskalne i średniookresowy plan budżetowo-strukturalny.

**Anotacja operatora:** reguły krajowe są arbitralne, więc nie mogą być głównym dowodem nierealizmu.

**Co było słabe wcześniej:** dowód nierealizmu opierał się zbyt mocno na prawie krajowym.

**Obecny fragment paperu:**

> Poland's domestic fiscal regime and medium term fiscal structural plan are consistent with this reading, but the arithmetic is the load-bearing point: the baseline endpoint is a surveillance counterfactual under strained debt dynamics, not a fiscal path that the Polish government could select and sustain

**Dlaczego uznajemy to za zaadresowane głęboko:** czasownik zmieniono z "reinforce this interpretation" na "are consistent with this reading, but the arithmetic is the load-bearing point". Reżim krajowy i plan średniookresowy są teraz tłem, nie dowodem.

**Widoczne dowody i źródła:** ten sam warunek ECB WP2486 i wejścia DSM2025. Zmiana udokumentowana w `proposals/stream1_commission_baseline_proposal.md` punkt 7.

**Walidacja Pro:** wymiar A (arytmetyka) PASS, wszystkie liczby pod argumentem się odtwarzają.

**Ograniczenie:** brak.

**Status:** zamknięte po Pro 10/10.

# Klaster B: krytyka Borys, Ciżkowicz, Rzońca, szeroka nie tylko o inwestycjach

## B1 (M10, N03, R953-G3a): krytyka poszerzona na cały claim ekspansywnej austerity

**Podkreślenie operatora:** zdanie traktujące pracę jako wąską instancję tezy tylko dla pytania o inwestycje publiczne.

**Anotacja operatora:** krytyka ma być szeroka i miażdżąca, przez wszystkie kanały, które autorzy wskazują, nie tylko o cięciach inwestycji.

**Co było słabe wcześniej:** zdanie zawężało krytykę do pytania o inwestycje publiczne.

**Obecny fragment paperu:**

> Borys, Ciżkowicz and Rzońca (2013) advance the expansionary-austerity claim across the full set of demand components on which that claim depends, and this paper rejects it on each of those components rather than only for public investment. Their New Member State panel identifies fiscal impulses through four aggregate procedures and reports that expenditure-based fiscal adjustments are accompanied by accelerated private investment and export growth, stronger wage moderation, and improved cost competitiveness, whereas expenditure-based fiscal stimuli decelerate private investment and export growth and weaken competitiveness (Borys, Ciżkowicz and Rzońca, 2013).

**Dlaczego uznajemy to za zaadresowane głęboko:** krytyka obejmuje teraz cały claim ekspansywnej austerity przez cztery kanały, które sami autorzy wskazują, czyli inwestycje prywatne, eksport, moderację płac i konkurencyjność kosztową. Stara rama "narrow instance" i koncesja "rather neutral" zostały usunięte.

**Widoczne dowody i źródła:** Borys, Ciżkowicz i Rzońca (2013), NBP WP 161, dosłowne przyznania autorów z dossier (NBP161 linie 241-245, 563-566, 991-996, 1014-1016). Kotwica odwrotnej przyczynowości z Breuer (2019).

**Walidacja Pro:** wymiar B (wierność cytatów) PASS, pięć dosłownych cytatów Borysa potwierdzonych wobec pliku źródłowego.

**Ograniczenie:** brak bezpośredniej opublikowanej krytyki Borysa et al. z nazwy w kanonie, wsparcie jest bezpośrednie dla metod i analogiczne dla szerszej literatury.

**Status:** zamknięte po Pro 10/10.

## B2 (N02, R953-G2, F06): usunięta koncesja "rather neutral", brak pozytywnego statusu

**Podkreślenie operatora:** słowo evidence i fraza "described as rather neutral".

**Anotacja operatora:** określenie zbyt pozytywne, zdanie nie może sugerować, że krytykowana praca ma rację nawet w wąskim sensie, oraz brak długich myślników w okolicy.

**Co było słabe wcześniej:** poprzednie zdanie nadawało tezie lokalnie pozytywny status przez koncesję "rather neutral".

**Obecny fragment paperu:**

> The authors read the small estimated effect on aggregate GDP not as a refutation but as confirmation, since in their account expenditure cuts shift growth toward investment, exports, and the cost channel; the claim that cutting expenditure stimulates private investment, exports, and competitiveness is therefore the operative expansionary-austerity proposition, and it is that proposition this paper rejects.

**Dlaczego uznajemy to za zaadresowane głęboko:** koncesję usunięto. Bliski zera efekt na zagregowany PKB jest teraz przedstawiony jako część tezy samych autorów, nie jako fakt na ich korzyść. Zdanie nie przyznaje pozytywnego statusu nawet lokalnie.

**Widoczne dowody i źródła:** wniosek NBP161, dosłownie linia 1192-1193 ("the total output response to fiscal policy is shaped mainly by the reaction of investment and export"). Zmiana w `proposals/stream1_borys_proposal.md` punkt 2.

**Walidacja Pro:** wymiar B (wierność cytatów) PASS oraz higiena długich myślników PASS, manuskrypt ma zero długich myślników i półpauz.

**Ograniczenie:** artykuł zostaje w paperze jako istotny dla debaty o ekspansywnej austerity, zmieniono jego status interpretacyjny.

**Status:** zamknięte po Pro 10/10.

## B3 (R953-G3b): żargon rozwinięty w prostym języku przy pierwszym użyciu

**Podkreślenie operatora:** skróty CAPB, von Hagen, action-based dataset, CAPB-type.

**Anotacja operatora:** rozwinąć albo usunąć te terminy przy pierwszym użyciu, prosty język.

**Co było słabe wcześniej:** gołe tokeny żargonowe bez wyjaśnienia.

**Obecny fragment paperu:**

> The identifiers are the cyclically-adjusted primary balance (the budget balance net of interest, purged of the part of the deficit that moves automatically with the business cycle, abbreviated CAPB), the underlying balance (the CAPB further corrected for one-off transfers), an impulse derived from the simplified growth-accounting rule associated with von Hagen, and a reduced action-based indicator that records only the sign of legislated fiscal action rather than its size.

**Dlaczego uznajemy to za zaadresowane głęboko:** każdy termin jest teraz glosowany prostym językiem przy pierwszym użyciu, a goły token "CAPB-type indicators" przeredagowano na opisową frazę.

**Widoczne dowody i źródła:** kotwice liniowe w `proposals/stream1_borys_proposal.md` punkt 3 (CAPB 555-558, underlying balance 563-566, von Hagen 570-571, reduced action-based 612-628).

**Walidacja Pro:** wymiar B (wierność cytatów) PASS, proza niosąca te rozwinięcia bez błędnej atrybucji.

**Ograniczenie:** brak.

**Status:** zamknięte po Pro 10/10.

## B4 (R953-G3c): trzy zarzuty oparte na dosłownych przyznaniach autorów, widoczna głębia

**Podkreślenie operatora:** trzy zarzuty przeciw przenoszeniu Borysa na cięcia inwestycji.

**Anotacja operatora:** czy te argumenty są mocne, czy mamy literaturę na ich poparcie, proszę pogłębić, poszerzyć kanon, dodać odniesienia.

**Co było słabe wcześniej:** trzy intuicyjne zdania bez widocznej mapy źródło do twierdzenia.

**Obecny fragment paperu:**

> The result cannot support claims about cutting public investment for three reasons, and the strongest version of each reason is one the authors themselves state. First, the fiscal impulses rest on aggregate balance measures and an action-based proxy that mix expenditure instruments together and never isolate public investment. The authors qualify the CAPB themselves, noting that it "should be used with caution, as noticed by the IMF (2010)". Second, the timing of consolidation episodes is exposed to the selection problem that the authors concede they cannot remove. They write that controlling for endogeneity through fiscal impulses "may be insufficient to fully eliminate the endogeneity bias", that an instrumental-variables estimator is barred because "the severe bias of this estimator when applied to short samples prevent us from using it", and that the results "should be treated with caution because of the estimation problems typical for panel data models". Third, every channel the authors propose runs through wage moderation, cost competitiveness, private investment, and exports, none of which is public capital formation. The authors close on the same note, conceding that "the conclusions drawn on their basis should be taken with caution".

**Dlaczego uznajemy to za zaadresowane głęboko:** każdy z trzech zarzutów stoi teraz na dosłownym przyznaniu samych autorów z NBP WP161, zakotwiczonym w konkretnych liniach źródła. Najmocniejsza wersja każdego zarzutu pochodzi od krytykowanej pracy.

**Widoczne dowody i źródła:** dossier Ognisko 2, dosłowne cytaty z NBP161 (linie 241-245, 991-996, 563-566, 1014-1016). Zmiany w `proposals/stream1_borys_proposal.md` punkty 4-6.

**Walidacja Pro:** wymiar B (wierność cytatów) PASS, wszystkie pięć cytatów Borysa potwierdzone dosłownie, łącznie z gramatyką źródła.

**Ograniczenie:** podparcie jest bezpośrednie dla metod artykułu i analogiczne dla szerszej literatury identyfikacyjnej.

**Status:** zamknięte po Pro 10/10.

# Klaster C: krytyka Alesiny, ogólna nie zawężona

## C1 (M09): usunięta koncesja "useful", zarzut identyfikacyjny uogólniony na całą literaturę

**Podkreślenie operatora:** zdanie "this categorization is useful for broadly comparing adjustment styles".

**Anotacja operatora:** usunąć koncesję, uogólnić zarzut identyfikacyjny na całą literaturę, nie tylko tę pracę.

**Co było słabe wcześniej:** koncesja "useful" i zawężenie zarzutu do jednej pracy.

**Obecny fragment paperu:**

> The identification problem here is not specific to one study but runs through this entire line of work: aggregate plans are not fiscal instruments, and plan labels are not shocks. The originators of this literature concede the gap themselves. Alesina and Ardagna (2010) acknowledge that "there can still be an endogeneity issue related to the occurrence of fiscal adjustments and expansions, because, in principle, discretionary policy choices of fiscal authorities can be affected by countries' macroeconomic conditions", and that the correlation between a successful adjustment and a falling debt ratio "is not perfect" because the numerator can drop faster than the denominator.

**Dlaczego uznajemy to za zaadresowane głęboko:** koncesję "useful" usunięto, a zarzut identyfikacyjny rozszerzono na całą linię badań przez własne przyznania twórców (Alesina i Ardagna 2010), reapraisal flagowych epizodów u Perottiego (2011) i poziom pomiaru u Breuera (2019). Inwestycje publiczne zostają jako przypadek decydujący, nie jako jedyny zakres.

**Widoczne dowody i źródła:** dossier ognisko 3 (Alesina-Ardagna 2010 linie 349-352 i 495-498, Perotti 2011 linie 50-57 i 137-139, Breuer 2019 linie 114-119 i 245-247). Zmiany w `proposals/stream1_alesina_proposal.md`.

**Walidacja Pro:** wymiar B (wierność cytatów) PASS, wszystkie dziesięć cytatów sekcji 1.2 potwierdzone.

**Ograniczenie:** brak.

**Status:** zamknięte po Pro 10/10.

## C2 (pillar-2): zarzut utrzymany ogólny, bez ponownego zawężania do inwestycji

**Podkreślenie operatora:** zdanie o cięciach wydatków, zwłaszcza inwestycji, poprawiających dług.

**Anotacja operatora:** utrzymać ogólność zarzutu, nie zawężać z powrotem do inwestycji publicznych.

**Co było słabe wcześniej:** zamknięcie zarzutu z powrotem na inwestycje publiczne.

**Obecny fragment paperu:**

> Evidence on the composition of consolidation therefore does not separate one expenditure instrument from another when evaluating the macroeconomic consequences of fiscal adjustment. For the question studied here this gap is decisive, because public investment is precisely the instrument that aggregate composition labels submerge, which is why the analysis below measures movements in public investment directly and traces their dynamic output responses (Alesina, Favero and Giavazzi, 2015; Breuer, 2019; Ardanaz, Cavallo, Izquierdo and Puig, 2021).

**Dlaczego uznajemy to za zaadresowane głęboko:** zdanie końcowe uogólniono z wąskiego "does not cleanly separate public investment from public consumption" na "does not separate one expenditure instrument from another". Inwestycje publiczne są teraz stawką tej pracy, nie zakresem zarzutu.

**Widoczne dowody i źródła:** `proposals/stream1_alesina_proposal.md` punkt 10, oparte na cytacie Breuera (2019) o odwrotnej przyczynowości CAPB.

**Walidacja Pro:** edycja prozy, walidowana przez wierność cytatów PASS dla sekcji 1.2 i ogólny werdykt manuskryptu 10/10.

**Ograniczenie:** brak.

**Status:** zamknięte po Pro 10/10.

# Klaster D: weryfikacja źródeł i atrybucji

## D1 (F10): pozycja Grodzicki, Możdżeń, Zygmuntowski sprawdzona u źródła i poprawiona

**Podkreślenie operatora:** pozycja "Grodzicki, Mozdzen and Zygmuntowski (2022) support the fiscal-rule part".

**Anotacja operatora:** sprawdzić, czy ci autorzy w tym kontekście to napisali, bo kanon ma to jako monografię, a nie angielski policy report.

**Co było słabe wcześniej:** zmyślony angielski tytuł "policy report" w pozycji bibliograficznej.

**Obecny fragment paperu:**

> Grodzicki, M., Mozdzen, M. and Zygmuntowski, J. J. (2022). Numeryczne reguly fiskalne - podejscie krytyczne [Numerical fiscal rules: a critical approach]. In Polityka fiskalna dla regeneracji. Warszawa: Wydawnictwo Naukowe Scholar.

**Dlaczego uznajemy to za zaadresowane głęboko:** atrybucja trzech autorów i teza rozdziału potwierdzone u źródła. R955 zastąpił zmyślony angielski tytuł faktycznym rozdziałem polskiej monografii. Dodatkowo, w tej rundzie wykryto i poprawiono drobny błąd tytułu: monografia nosi tytuł "Polityka fiskalna dla regeneracji" (z "dla"), potwierdzony stroną kanonu wiki i numerem ISBN 978-83-66849-44-1; manuskrypt miał wcześniej "Polityka fiskalna regeneracji" bez "dla", co teraz naprawiono.

**Widoczne dowody i źródła:** `audit/AUDIT_REPORT_STREAM2_SOURCES_20260603.md`, strona kanonu `wiki/literature/mozdzen-zygmuntowski-2022.md` (pełny tytuł i ISBN).

**Walidacja Pro:** wymiar B (wierność cytatów) PASS, brak błędnej atrybucji w warstwie literatury. To jest parafraza, nie jeden z dziesięciu dosłownych cytatów.

**Ograniczenie:** brak, po poprawce tytułu pozycja jest zgodna ze źródłem.

**Status:** zamknięte po Pro 10/10, z poprawką tytułu w tej rundzie.

## D2 (N04, R953-G4, M18): termin "conditioning information set" zachowany jako termin z literatury

**Podkreślenie operatora:** "conditioning information set", "conditioning dimension".

**Anotacja operatora:** sprawdzić, czy "conditioning set" to termin z literatury lokalnych projekcji, przywrócić i ujednolicić jeśli tak, uprościć jeśli nie.

**Co było słabe wcześniej:** wcześniejsze rozliczenie nie pokazało, czy literatura używa takiego języka.

**Obecny fragment paperu:**

> For fiscal multiplier analysis the method is well suited, since the estimate depends on the shock definition, the fiscal instrument, the horizon, and the conditioning information set (Ramey and Zubairy, 2018; Ramey, 2019).

**Dlaczego uznajemy to za zaadresowane głęboko:** termin jest używany w pokrewnej literaturze lokalnych projekcji, więc zachowano go w paperze i ujednolicono rodzinę terminów warunkujących w sekcjach 2.1 i 2.2. Uczciwie: w samych Ramey-Zubairy 2018 potwierdzony jest koncept (mnożniki zależą od stanów, na które się warunkuje), a sam dosłowny zwrot pojawia się u Cloyne, Jorda i Taylor oraz Dell'Erba, Koloskova i Poplawski-Ribeiro. Termin został w paperze zachowany, nie usunięty i przywrócony.

**Widoczne dowody i źródła:** Ramey i Zubairy (2018) przypis 10, oraz `proposals/stream4_style_pilot.md` linia 95 i kontrola niezmiennika linia 114, gdzie termin jest na liście zachowanych bez zmiany.

**Walidacja Pro:** nie był osobno adjudykowany jako wymiar, walidowany pośrednio przez ogólny werdykt 10/10.

**Ograniczenie:** termin jest dopuszczalny w literaturze, choć mniej przyjazny czytelnikowi.

**Status:** zamknięte po Pro 10/10.

## D3 (F11): kanał kursowy i kompozycyjny ma źródło w kanonie i jest obecny

**Podkreślenie operatora:** materiał o kursie walutowym i kompozycji usunięty z powodu braku źródła.

**Anotacja operatora:** nie usuwać, doszukać źródła w kanonie i przywrócić, jeśli istnieje.

**Co było słabe wcześniej:** ryzyko usunięcia materiału bez sprawdzenia kanonu.

**Obecny fragment paperu:**

> This pattern fits the trade multiplier literature, which treats import leakage as composition dependent rather than governed by a simple openness rule: fiscal transmission depends on the domestic value added content of demand, the relative import content of public versus private expenditure, production structure, financing, and invoicing conditions (Ilzetzki, Mendoza and Vegh, 2013; Cacciatore and Traum, 2020; Crespo Cuaresma and Glocker, 2023).

**Dlaczego uznajemy to za zaadresowane głęboko:** audyt źródeł potwierdził, że źródło istnieje w kanonie (Ilzetzki, Mendoza i Vegh 2013, mnożniki różne według reżimu kursowego i kompozycja wydatków istotna). Materiał jest obecny i zacytowany, nie usunięty.

**Widoczne dowody i źródła:** `audit/AUDIT_REPORT_STREAM2_SOURCES_20260603.md` sekcja F11, pozycje bibliograficzne Ilzetzki-Mendoza-Vegh 2013, Cacciatore-Traum 2020, Crespo Cuaresma-Glocker 2023.

**Walidacja Pro:** wymiar F (higiena paczki) PASS i wymiar B PASS, `source_inventory_r788.csv` z 15 pozycjami obecny, źródło zamknięte.

**Ograniczenie:** dokładne sformułowanie zostaje decyzją operatora, materiał jest osadzony w kanonie.

**Status:** zamknięte po Pro 10/10.

## D4 (R02): cytowanie Ciaffi wskazuje właściwy paper

**Podkreślenie operatora:** cytat i link Ciaffi.

**Anotacja operatora:** potwierdzić, że cytowanie Ciaffi wskazuje właściwy paper.

**Co było słabe wcześniej:** ryzyko kolizji trzech różnych prac Ciaffi 2024.

**Obecny fragment paperu:**

> This shock-identification-plus-local projection structure follows Ciaffi, Deleidi and Di Domenico (2024), and the present paper adapts it to an EU27 annual panel and to the evaluation of Polish state variables.

**Dlaczego uznajemy to za zaadresowane głęboko:** manuskrypt nosi trzy odrębne prace Ciaffi 2024, każda przypisana poprawnie. Szkielet metodyczny cytuje Ciaffi, Deleidi i Di Domenico (2024, Journal of Policy Modeling), wyniki mnożnika OECD cytują Ciaffi, Deleidi i Capriati (2024, Economia Politica), a argument o predeterminacji dodaje Ciaffi, Deleidi i Mazzucato (2024, Industrial and Corporate Change). Żadne cytowanie nie koliduje z niewłaściwą pracą.

**Widoczne dowody i źródła:** lista referencji manuskryptu, trzy odrębne pozycje Ciaffi 2024 z własnymi współautorami i czasopismami.

**Walidacja Pro:** brak błędnej atrybucji Ciaffi w R962, wymiar B (wierność cytatów) PASS bez wytkniętej wady proweniencji.

**Ograniczenie:** brak.

**Status:** zamknięte po Pro 10/10.

# Klaster E: treść merytoryczna, sekcja aplikacji

## E1 (F13, M22): Konin jako dowód cięcia inwestycji, krytyka nie za słaba

**Podkreślenie operatora:** CPK i Konin jako przykłady.

**Anotacja operatora:** Konin ma być dowodem cięć inwestycji, a krytyka ograniczania programu przez rząd nie ma być za słaba, bo formalnie program trwa, materialnie tną.

**Co było słabe wcześniej:** ryzyko zbyt słabego sformułowania, że program trwa formalnie, a jest materialnie cięty.

**Obecny fragment paperu:**

> Moving from a committed implementation route with a designated partner back to renewed site analysis is itself a substantial investment cut behind formal programme continuity, alongside delayed investment decisions and a slower annual expenditure trajectory.

**Dlaczego uznajemy to za zaadresowane głęboko:** Konin jest wprost ujęty jako istotne cięcie inwestycji, a CPK i program jądrowy jako formalna ciągłość z materialnym ograniczeniem. Edycje stylu obniżyły rejestr bez osłabiania tezy, użyto słów "falls sharply", "cut", "substantial investment cut".

**Widoczne dowody i źródła:** własny zestaw źródeł oficjalnych sekcji aplikacji (uchwały Rady Ministrów 2023/2024, Ministerstwo Aktywów Państwowych 2022, Ministerstwo Energii 2025, Yonhap 2025, Centralny Port Komunikacyjny 2025). Podstawa edycji: `proposals/stream4_b5.json` pozycje 1-2.

**Walidacja Pro:** wymiar D (integralność wywodu) potwierdził, że ledger stylu ma 16 pozycji, wszystkie nowe wersje obecne, stare nieobecne, bez regresji liczb ani konkluzji. Ogólny werdykt manuskryptu 10/10.

**Ograniczenie:** brak.

**Status:** zamknięte po Pro 10/10.

# Sekcja procesowa: F09 i R953-G3d

**Anotacja operatora F09:** "To jest cytat?!" przy fragmencie w dokumencie rozliczeniowym.

**Anotacja operatora R953-G3d:** dokument oznaczony "Status przed Pro" trafił do operatora przed audytem Pro.

**Co było słabe wcześniej:** to są uwagi o dokumencie rozliczeniowym i dyscyplinie procesu, nie o prozie manuskryptu. Weryfikacja potwierdziła, że operator miał rację co do F09: poprzednie rozliczenie niosło cytat przypisany do sekcji, którego brzmienie nie zgadzało się z żywym manuskryptem. To był realnie źle dopasowany cytat.

**Jak to zamknięto:** ten dokument używa wyłącznie cytatów dosłownych z żywego manuskryptu, a każdy został niezależnie sprawdzony pod kątem obecności w pliku. Cała praca tej rundy przeszła przez pełny audyt Pro przed jakąkolwiek dostawą, więc żaden materiał oznaczony "przed Pro" nie idzie do Ciebie jako zamknięty. Status każdego punktu wyżej brzmi "zamknięte po Pro 10/10", a nie "przed Pro".

**Status:** zamknięte przez dyscyplinę procesu, nie przez edycję manuskryptu.

# Pozycje zweryfikowane jako już domknięte

Trzy wcześniejsze pozycje sprawdzono bezpośrednim przeszukaniem żywego manuskryptu i nie mają w nim śladu, więc nie wymagały edycji:

- M08 i F04 (wzmianki o notebooku i materiałach replikacyjnych): zero trafień frazy "notebook" w prozie manuskryptu.
- M21 ("midpoint to nie average"): zero trafień frazy "midpoint".
- M24 (kolumna "Design matrix rank"): zero trafień "design matrix" ani "matrix rank" w prozie, jedyne "rank" to zapis matematyczny w appendixie.

**Status:** zweryfikowane jako nieobecne w manuskrypcie, domknięte.

# Bramka głębokości

Każdy punkt wyżej przeszedł podwójną kontrolę: ugruntowanie w dosłownym fragmencie żywego manuskryptu oraz adwersaryjną weryfikację, czy odpowiedź rzeczywiście trafia w sens anotacji, czy nie jest płytka, czy nie przyznaje pozytywnego statusu krytykowanej tezie i czy nie zawęża z powrotem. Wszystkie piętnaście punktów przeszło obie kontrole. Pełny audyt Pro zwrócił 10/10 dla manuskryptu i 10/10 dla notebooka bez wymaganych poprawek.
