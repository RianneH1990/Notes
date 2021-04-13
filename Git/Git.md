#GIT

###Git basics
1. Maak een nieuw project aan.
2. Maak een .gitignore bestand aan.
3. Zorg er voor dat de /.idea folder wordt genegeerd. 
4. Open de terminal en typ git init om een git bestand aan te maken locaal.
5. Maak een pagina aan, bijv. index.html.
6. Typ git status om te checken of er al iets is opgeslagen.
7. Track je veranderingen op je pagina met git add "index.html" of git add . (om alles te toevoegen).
8. Maak een git commit om de veranderingen te commiten: git commig -m "omschrijving van commit".
9. Check jezelf met git status.
10. Git add en commit zo vaak mogelijk in het maken van de code zodat er een goede documentatie is van wat je veranderd in de code.
11. Maak in Github een nieuwe repository aan. Geef deze de naam van het project waar je aan werkt.
12. VOEG GEEN readme.md, license en .gitignore toe.
13. Check als je je project hebt gecloned check dan altijd of er niet nog een andere repository gelinked is, met git remote -v. 
14. Als er nog een oude koppeling is, verwijder deze met git remote remove origin.
15. Voeg je gemaakte repository toe met de link in Github.
16. Push je code naar de repo met git push origin main/master
17. Check of de koppeling goed is gegaan door f5 (de pagina refreshen) op je github.
    
###Git branch aanmaken
1. Clone het project waar je aan wilt werken.
2. Verwijder de bestaande repository link met git remote remove origin.
3. Koppel je eigen repository er aan.
4. git checkout -b "naam van branch"
5. git push origin "naam van branch"

###Pull request
1. Maak een nieuwe branch aan in je project.
2. verander, add, commit en push je veranderingen naar de branch.
3. Maak bij Github een nieuwe pull request aan.
4. Check of alle content in de pull request staat.
5. Na het terugkrijgen van feedback/aanpassen na feedback kun je via Github de branch weer samen voegen met de main. Door te mergen.

   