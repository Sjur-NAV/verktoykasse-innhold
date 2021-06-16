# Verktøykasse innhold

## Reserverte mappe-navn
`designsystem`
`components`
`resources`
`patterns`
`accessibility`

## Hvordan legge til innhold

Denne løsningen støtter bare Markdown filer. Dette vil si filer som ender med ".md".
> For en liten how-to for hvordan man skriver markdown: https://www.markdownguide.org/basic-syntax

### Ny underkategori under design.nav.no

Lag en ny mappe på toppnivå i repoet slik som "metoder" her:

![Screenshot 2021-06-16 at 18 31 25](https://user-images.githubusercontent.com/26967723/122258357-3f467180-ced1-11eb-9916-233500efd849.png)


Innholdet under mappen i eksemplet vil da bli lagt under design.nav.no/metoder,
hvis du lager en mappe med navn eks "sidemaler", så vil innholdet bli lagt under design.nav.no/sidemaler 

For å gjøre dette kan man trykke på "create new file" slik som eksemplet her: 


![Screenshot 2021-06-16 at 18 36 43](https://user-images.githubusercontent.com/26967723/122259361-65204600-ced2-11eb-912f-0d601f611f4b.png)


Man vil da få opp github sin editor. Man kan ikke lage tomme mapper i github, så man må lage en fil i tillegg når den opprettes.
Dette gjøres ved å skrive mappenavn/filnavn.md

I eksemplet under vil det her bli opprettet en mappe "sidemaler" med filen "readme.md"
![Screenshot 2021-06-16 at 18 44 52](https://user-images.githubusercontent.com/26967723/122259906-f68fb800-ced2-11eb-9026-452d734d3f71.png)


### Strukturerning av innhold

Løsningen støtter bare **1** nivå for nå, dette vil si at man ikke kan nøste mapper slikt: "/sidemaler/produktsider/side-1.md".

I hver mappe regnes filen med navn "readme.md" som "forsiden" til denne underkategorien. Dette vil si at "sidemaler/readme.md" vil vises på design.nav.no/sidemaler

Andre filer som har eks navn: "side-1.md" vil da ligge på design.nav.no/sidemaler/side-1. 

**Bare filer med formatet: "side 1.md" eller "side-1.md" er mulig.**

### Innhold i hver fil

I hver fil må man legge med litt ekstra info slik at menyen vet hva som skal stå der. Dette gjør man ved på legge til tre linjer med kode.
I eksemplet under forteller man siden at det skal stå "Hjem" i sidemenyen som linker til denne siden
```
---
title: Hjem
---
```

Eksemplet under vil ha en sidetittel, en undertittel med tekstinnhold under. I tillegg så vil linken i sidemenyen si "Maler"

```markdown
---
title: Maler
---

# Tittel som vises øverst på siden (<h1>)

## Undertittel (<h2>)

Tekstblokk som vil bli lagt under undertittellen (<p>)
```

## Hvordan jobbe med innhold

Når man lager en ny fil eller mappe kan man ikke bare pushe dette rett på prod. Istedenfor må man opprette en pull-request slik som eksemplet: 
![Screenshot 2021-06-16 at 19 13 14](https://user-images.githubusercontent.com/26967723/122263797-1f19b100-ced7-11eb-9a4e-25b3aa37c277.png)

Da får andre muligheten til å verifisere at innholdet ser greit ut før det merges og sendes til prod. man kan også lage det som en "draft pr" hvis det er mye som må fikses før det trenger å bli godkjent.

Man kan da velge "branchen" som pull requesten ligger på for å jobbe videre med innholdet før man vil kjøre det ut i prod (her vil det være "sidemaler").
![Screenshot 2021-06-16 at 19 18 46](https://user-images.githubusercontent.com/26967723/122264596-ff36bd00-ced7-11eb-9e2b-7242f4114fd7.png)




## Kontakt

Ken Aleksander Johansen på Slack
