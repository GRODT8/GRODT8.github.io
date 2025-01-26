# GRODT Kleding Webshop

Welkom bij de **GRODT Kleding Webshop**! Deze website is een moderne, stijlvolle en minimalistische webshop voor het merk GRODT, wat staat voor *"Get Rich Or Die Trying"*. De webshop is gebouwd met HTML, CSS en JavaScript en is eenvoudig uit te breiden of te hosten.

## Inhoud
1. [Functies](#functies)
2. [Installatie](#installatie)
3. [Gebruik](#gebruik)
4. [Structuur](#structuur)
5. [Hosting op GitHub Pages](#hosting-op-github-pages)
6. [Contact](#contact)

## Functies
- **Moderne layout**: Een strakke, responsieve interface met TailwindCSS.
- **Productoverzicht**: Dynamisch gegenereerde producten uit een lijst.
- **Winkelwagen-knop**: Placeholder voor toekomstige winkelwagenfunctionaliteit.
- **Heldere structuur**: Geschikt voor uitbreidingen en aanpassingen.

## Installatie

Volg deze stappen om de website lokaal te draaien:

1. **Clone de repository**:
   ```bash
   git clone https://github.com/<jouw-gebruikersnaam>/grodt-webshop.git
   ```

2. **Open het project**:
   Ga naar de map waar je het project hebt gekloond.

3. **Start de applicatie**:
   Open het bestand `index.html` in een browser.

## Gebruik

De website is ontworpen om eenvoudig aanpasbaar te zijn. Je kunt de productenlijst vinden in de JavaScript-code:
```javascript
const products = [
  {
    id: 1,
    name: "GRODT Hoodie",
    price: "€59,99",
    image: "https://via.placeholder.com/300x400",
  },
  {
    id: 2,
    name: "GRODT T-Shirt",
    price: "€29,99",
    image: "https://via.placeholder.com/300x400",
  },
  // Voeg meer producten toe hier...
];
```
Je kunt nieuwe producten toevoegen door een nieuw object aan deze lijst toe te voegen.

## Structuur

De bestanden en mappen zijn als volgt gestructureerd:
```
/
├── index.html       # Hoofdbestand voor de webshop
├── styles.css       # TailwindCSS-achtige styling
├── script.js        # JavaScript-logica voor dynamische content
└── assets/          # Afbeeldingen en andere media (optioneel)
```

## Hosting op GitHub Pages

1. **Commit en push je code** naar GitHub.
2. Ga naar de repository-instellingen en zoek naar **GitHub Pages**.
3. Selecteer de branch en root-map waar je `index.html` zich bevindt.
4. Je website is nu live op `https://<jouw-gebruikersnaam>.github.io/grodt-webshop`.

## Contact

Voor vragen of opmerkingen over dit project kun je contact opnemen via:
- **E-mail**: support@grodt.com
- **Instagram**: [@grodt_clothing](https://instagram.com/grodt_clothing)

---

Bedankt voor het gebruiken van de GRODT Kleding Webshop. We hopen dat je webshop een groot succes wordt!

