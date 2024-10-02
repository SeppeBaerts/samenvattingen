# Devops

## Agile DevOps and the 3 ways

> agile en devops is was ik deze git shizzle aan't uitzoeken, it did not work.

### The 3 Ways

#### Principles of flow (First Way)

Go with the flow, je de bedoeling is dat je van A naar B flowed. Je kunt dit op verschillende manieren doen. Waterfall,
boven naar beneneden?

Hier gaat het ook over een pipeline => Devops automatisch laten unit testen etc
> Ja was even verloren, moet je de dia's nog eens nakijken.

#### Principles of feedback (Second way)

Je krijgt direct feedback wanneer je iets pushed. Werken de Unit testen? Zijn er problemen met dependency's?...

Hoe gaan we die feedback weergeven? Door continue monitoren & testen maken,...
Feedback zit bijvoorbeeld ook als je een pull request stuurt,... Test alles op het moment dat het kan, dat is vooral
belangrijk.

Continues integration => Zorgen dat je de demo status continu kunt valideren door automatische testen. Vanaf het moment
dat zo een test failed, zal de pipeline of productielijn ook meteen stop gezet worden.

Digital Andon cord => Wanneer er iets mis loopt stop je met features toevoegen en los je eerst het probleem op. Angular
is hier heel erg in de mist door gegaan. Die is features blijven uitpompen en op een moment konden ze niks meer doen
omdat die core zo buggy was. Hierdoor hebben ze angular terug van de ground-up moeten maken. Als ze nu in het begin meer
moeite hadden gedaan om een "sprint-stop" in te plannen zodat iedereen even aan de problemen werkte zou dat niet
begonnen.

Manueel testen is niet goed aangezien je dit pas op het einde van de productielijn kunt doen. Bij geautomatiseerd
testen, moet je alleen maar de nieuwe feautures testen en hier dan ook meteen Automated unit testen schrijven. Hierdoor
krijg je meteen feedback en moet je niet continu alles opnieuw manueel testen.

#### Organasation Culture (Third way)

De dynamica van een bedrijf is heel belangrijk, iedereen moet het gevoel hebben dat ze een inspraak hebben (of toch het
gevoel),... Hier sommen ze 4 dingen op

source: https://dzone.com/articles/is-devops-agile

- Enable safety (het moet veilig zijn om je eigen mening te zeggen)
- Improvement of daily work
- Local discoveries to global improvements. (als er een goed idee is, hou het dan niet voor jezelf maar zorg dat de
  groep beter wordt.)
- Inject Resilience.

Wat Wij vooral moeten meenemen is dat je moet durven falen, het falen is ook een zeer grote leerkans.

### Agile vs scrum

Honestly ze zijn heir eerder gewoon de dia aan't overlezen, dus ik ga hier gewoon even de image inzette.
<img src="devops-to-agile-infographics.png" alt="Infographics over devops."/>

## Source control

### Waarom Source control

Geen vingerwijs-cultuur, maar wel weten wat er gebeurd is. Niet wie is het geweest, maar wel wat is er gebeurd.

Gewoon zodat je niet hotfix op hotfix had.

### Recap & Algemeen gebruik

Versie beheer => Wordt gebruikt voor versiebeheer van alle tekstdocumenten. In principe alles wat niet binary is, maar
ze zeggen ook net dat binary wel werkt... Maar aan de andere kant, sommige testfiles zijn toch ook binary, I guess dat
ze het momenteel hebben over de veranderingen tracken.

#### Github en Collaborations 

 