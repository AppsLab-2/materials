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
  2. Napíš čo robia zmeny, ktoré sa chystáš commitnúť imperatívnym spôsobom
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
</details>
