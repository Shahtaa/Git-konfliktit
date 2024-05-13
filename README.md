# Git-konfliktit

# Luodaan uusi Git-repositorio tai käytetään olemassa olevaa

git init

# Luodaan main- ja develop-haarat

git branch main
git branch develop

# Siirrytään develop-haaraan

git checkout develop

# Luodaan koodia develop-haaraan

touch HelloWorld.java

# Tee muutoksia tiedostoon HelloWorld

public class HelloWorld {
public static void main(String[] args) {
System.out.println("Hello, World!");
}
}

# Lisätään .gitignore-tiedosto

nano .gitignore

# Luo tai muokkaa .gitignore-tiedostoa ja lisää siihen tarvittavat tiedostot ja hakemistot, joita ei haluta lisätä Git-repositorioon.

# Tehdään triviaali merge

git checkout main
git merge develop

# Tehdään muutoksia molemmissa haaroissa, jotka aiheuttavat konflikteja

# Testataan konfliktien syntyminen

git merge develop

# Ratkotaan mahdolliset konfliktit

# Kun konflikti ilmenee, ratkaistaan se käyttäen haluamaamme työkalua, esimerkiksi Sourcetree + KDiff3.

# Poistetaan päähaara

git branch -d main
