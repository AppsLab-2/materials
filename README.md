# Tu nájdeš materiály, ktoré by ti mohli pomôcť

<details>
  <summary>Nastavenie svojho Git repozitára</summary>

  ### Vytvor si nový priečinok
  
  1. Choď do c/Users/openlab (alebo do nejakého iného podľa svojho uváženia)
  2. Vytvor priečinok s názvom appslab + aktuálny rok, napr. appslab2020
  3. Pokračuj podľa prezentácie **Git repo set up** v tomto repozitári
</details>

<details>
  <summary>Základná práca s Git-om</summary>
  
  ## Základné príkazy
  
  Všetko sa dá nájsť v Git dokumentácii ==> https://git-scm.com/doc
  
  ### Git checkout

  Príkaz slúži na prepínanie sa medzi jednotlivými vetvami (branch).
  
  **git checkout *[branch name]***
  
  ak vetva ešte neexistuje
  
  **git checkout -b *[branch name]***

  ### Git commit

  Slúži na nahratie zmien do repozitára.

  **git commit -m "commit message"**
  
  Ako písať commit message?
  1. Začni veľkým písmenom
  2. Napíš čo robia zmeny, ktoré sa chystáš commitnúť imperatívnym spôsobom, napr. Pridaj metódu na výpočet niečoho
  3. Na konci vety sa nedáva bodka, výkričník...proste nič
  4. Skús sa zmestiť do 50 znakov
  
  Príklad: **Pridaj metódu pre výpočet dĺžky trasy**
  
  ### Git push
  
  Update-ne remote repozitár.
  
  **git push**
  
  Pri prvom vykonávaní príkazu git push (keď chcem pushnúť vetvu, ktorá ešte nie je v remote repozitári) bude potrebné pustiť git push nasledovne:
  
  git push --set-upstream origin *[branch name]*

  Všetky tieto príkazy sa dajú používať priamo v Git Bash konzole. Ako tieto príkazy realizovať v Intellij Idea nájdete v prezentácii **Working with Git in Intellij** v tomto repoziári.
</details>

<details>
  <summary>New to Java</summary>

  ### Konvencie pre písanie Java programov
  https://www.oracle.com/java/technologies/javase/codeconventions-namingconventions.html
  
  ### Java tutorials
  https://docs.oracle.com/javase/tutorial/tutorialLearningPaths.html
  
  ### Syntax Java vs C#
  https://www.slideshare.net/Pednekar19/difference-between-java-and-c
</details>

<details>
  <summary>Na čo si dať pozor pri prepájaní FE s BE </summary>
  <br>
  Pri volaní HTTP requestu z FE cez HttpClient je potrebné s BE zjednotiť:<br><br>
  
   **Endpoint** - volaný z FE musí existovať aj na BE. Príklad: Ak mám na BE napr. endpoint announcement/all tak FE musí volať presne taký istý endpoint, teda announcement/all.<br><br>
   **Použitú HTTP metódu** - musí byť rovnaká. Príklad: Ak mám na BE definovaný daný endpoint ako GET tak potom aj z FE musím volať httpClient.get...<br><br>
   **Očakávaný objekt a objekt, ktorý sa posiela** - je potrebné aby názvy atribútov boli rovnaké. Inak sa to nebude vedieť spárovať. Príklad: Ak BE posiela na FE objekt, ktorý ma atribúty s názvom name, surname a age tak na FE musí byť tiež objekt s atribútmi name, surname a age. Presne rovnaké názvy.<br>Podobne to platí aj opačne, teda keď FE posiela objekt na BE. Toto je napríklad v prípade POST metódy. Príklad: Vo formulári na FE som vyklikal nový inzerát a chcem ho poslať na BE aby sa uložil do DB.<br><br>
   **Názvy parametrov** - ak potrebujete poslať nejaké parametre tak parametre s rovnakým názvom musia byť nadefinované aj na BE pri príslušnom endpointe
</details>
