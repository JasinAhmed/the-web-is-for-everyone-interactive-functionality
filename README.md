# Interactive Functionality – AD Connect Talent Award

## Beschrijving
Voor deze opdracht heb ik een interactieve en toegankelijke webapplicatie ontwikkeld voor AD Connect, gericht op de Talent Award pagina.

Het doel van deze applicatie is om bezoekers niet alleen genomineerden te laten bekijken, maar ook actief te laten deelnemen door reacties (posts) te plaatsen.

De applicatie is gebouwd met server-side rendering via `server.js`, waardoor de website ook goed werkt zonder JavaScript.

Live demo:  
https://the-web-is-for-everyone-interactive-zio9.onrender.com/

---

## Opdracht
Ontwerp en ontwikkel een interactieve toepassing die:
- Toegankelijk is voor iedereen  
- Werkt op verschillende apparaten  
- Progressive enhancement toepast  
- Interactie mogelijk maakt voor de gebruiker  

---

## Gebruik

De gebruiker kan:

- Genomineerden bekijken  
- Doorklikken naar een detailpagina  
- Een post/reactie plaatsen  
- Een post verwijderen  
- Navigeren via een hamburger menu  

### User story
Als gebruiker wil ik een reactie kunnen plaatsen bij een genomineerde, zodat ik mijn mening of support kan delen.

---

## Functionaliteiten

- Overzicht van genomineerden  
- Detailpagina per genomineerde  
- Post systeem (create)  
- Delete functie (remove posts)  
- Hamburger menu (mobile navigation)  
- Responsive design  
- Light mode en gedeeltelijke dark mode  
- Loading/UX verbeteringen  

---

## Technische keuzes

Tijdens dit project heb ik bewust gekozen voor:

### Server-side rendering
- Gebouwd met Node.js (`server.js`)
- Pagina’s worden dynamisch gegenereerd
- Werkt zonder afhankelijk te zijn van JavaScript

### Form-based interactie
- Posts worden verstuurd via HTML formulieren (POST requests)
- Werkt ook zonder JavaScript

### Delete functionaliteit
- Gebruikers kunnen posts verwijderen
- Houdt de pagina overzichtelijk

### Hamburger menu
- Voor betere gebruikerservaring op mobiel
- Werkt als enhancement met JavaScript

---

## Toegankelijkheid

Toegankelijkheid stond centraal in deze opdracht.

Ik heb daarom:

- Semantische HTML gebruikt  
- Formulieren gebouwd die werken zonder JavaScript  
- Progressive enhancement toegepast  
- Responsive design gebruikt  

De basisfunctionaliteit (zoals posts plaatsen) werkt zonder JavaScript.  
JavaScript voegt alleen extra interactie toe.

---

## Progressive Enhancement

De website is opgebouwd volgens het principe van progressive enhancement:

1. Basis (HTML + server)
   - Content zichtbaar
   - Posts werken via formulieren  

2. Verbetering (CSS)
   - Layout en design  

3. Enhancement (JavaScript)
   - Hamburger menu  
   - Extra interactie  

---

## Gebruikte technieken

### Frontend
- HTML (semantisch en toegankelijk)
- CSS (responsive en styling)
- JavaScript (interactie)

### Backend
- Node.js
- Server-side rendering (`server.js`)

### Functionaliteit
- POST requests (form handling)
- Basis CRUD:
  - Create → posts toevoegen  
  - Delete → posts verwijderen  

---

## Problemen en oplossingen

Tijdens het project liep ik tegen meerdere uitdagingen aan:

- Posts werden niet goed weergegeven  
  → Opgelost door server-side rendering correct te implementeren  

- Te veel reacties op de pagina  
  → Opgelost met een delete functie  

- Navigatie werkte niet goed op mobiel  
  → Opgelost met een hamburger menu  

- Dark mode nog niet volledig  
  → Dit ben ik nog aan het verbeteren  

---

## Installatie

1. Clone de repository:
```bash
git clone <jouw-repository-link>
