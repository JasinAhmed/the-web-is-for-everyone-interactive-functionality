# AD Connect Talent Award – Website

Een interactieve website voor de Talent Award van AD Connect. Bezoekers kunnen genomineerden bekijken én reacties plaatsen.

🔗 **Live website:** [Bekijk hier](https://the-web-is-for-everyone-interactive-zio9.onrender.com/)  
📁 **Repository:** [GitHub – JasinAhmed](https://github.com/JasinAhmed/the-web-is-for-everyone-interactive-functionality)

---

## Inhoudsopgave

- [Beschrijving](#beschrijving)
- [Huisstijl](#huisstijl)
- [Responsive](#responsive)
- [Kenmerken](#kenmerken)
- [Installatie](#installatie)
- [Bronnen](#bronnen)
- [Licentie](#licentie)

---

## Beschrijving

Voor deze opdracht heb ik een interactieve website gemaakt voor de Talent Award pagina van AD Connect. De opdrachtgever wilde dat bezoekers niet alleen konden kijken, maar ook echt iets konden doen op de website.

De website werkt ook zonder JavaScript, zodat iedereen hem kan gebruiken.

Tijdens deze sprint heb ik vooral geleerd hoe je data kunt versturen naar Directus via een formulier.

---

### Reactie plaatsen

De belangrijkste functie op de website is het plaatsen van een reactie bij een genomineerde.

- Je ziet hoeveel reacties er al zijn voordat je er zelf eentje plaatst
- Als er nog geen reacties zijn, staat er *"Er zijn nog geen reacties"*
- Na het plaatsen word je automatisch naar jouw reactie gestuurd

**Code:**
```
server.js – regels 114 t/m 153
https://github.com/JasinAhmed/the-web-is-for-everyone-interactive-functionality/blob/29ea30665cfedca1946bddbd897787aa99345e0a/server.js#L114-L153
```

### Reactie verwijderen

Je kunt je reactie ook weer verwijderen. Dit werkt via een formulier, dus ook zonder JavaScript.

**Code:**
```
server.js – regels 156 t/m 171
https://github.com/JasinAhmed/the-web-is-for-everyone-interactive-functionality/blob/29ea30665cfedca1946bddbd897787aa99345e0a/server.js#L156-L171
```

---

## Huisstijl

De website is gebaseerd op het design van AD Connect.

- Kleuren die passen bij de huisstijl van de opdrachtgever
- Duidelijke letters die goed leesbaar zijn
- Simpel en overzichtelijk, zodat de genomineerden de aandacht krijgen

---

## Responsive

De website is gemaakt voor mobiel eerst, omdat de meeste bezoekers de site op hun telefoon bekijken. Hij werkt ook gewoon op een desktop.

---

## Kenmerken

De website is gebouwd met:

- HTML, CSS en JavaScript
- Node.js en Express
- Liquid (voor de pagina's op de server)
- JSON
- Directus (voor de data en API)

### Animaties

Mensen die geen beweging op hun scherm willen, krijgen geen animaties te zien. Dit doe ik met de volgende CSS:

```css
@media (prefers-reduced-motion: no-preference) {
  .highlight {
    border: 2px solid black;
    transition: border 0.5s ease;
  }

  .highlight.fade {
    border-color: transparent;
  }
}
```

---

## Installatie

### Hoe zet je het op

```bash
# 1. Kloon de repository
git clone https://github.com/JasinAhmed/the-web-is-for-everyone-interactive-functionality.git

# 2. Ga naar de map
cd the-web-is-for-everyone-interactive-functionality

# 3. Installeer de packages
npm install

# 5. Start de server
npm start
```

De website is nu te zien op `http://localhost:3000`.

---

## Bronnen

- [Node.js documentatie](https://nodejs.org/en/docs)
- [Express documentatie](https://expressjs.com/)
- [Directus documentatie](https://docs.directus.io/)
- [LiquidJS documentatie](https://liquidjs.com/)
- [MDN – HTML formulieren](https://developer.mozilla.org/en-US/docs/Learn/Forms)
- [MDN – prefers-reduced-motion](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-reduced-motion)
- [CSS-Tricks – Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [npm – express](https://www.npmjs.com/package/express)
- [npm – liquidjs](https://www.npmjs.com/package/liquidjs)
- [npm – dotenv](https://www.npmjs.com/package/dotenv)
- [npm – node-fetch](https://www.npmjs.com/package/node-fetch)

---

## Licentie
This project is licensed under the terms of the [MIT license](./LICENSE).
