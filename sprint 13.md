# Sprint 13 Your Tribe For Life

## Week 1

### Maandag 2 september

**Leervragen:**

1. Hoe zet je een project op met frameworks?
2. Wat is svelte(kit) en hoe kan ik het gebruiken?
3. Wanneer gebruik je svelte(kit)?
4. Hoe render je data uit een Headless CMS door middel van een framework?
5. Hoe kan ik complexere JavaScript gebruiken?

#### Team Canvas

[Team Canvas](https://github.com/user-attachments/assets/f73bbf96-51a6-44db-b13d-dbb1a4c05121)

#### [Project board](https://github.com/users/Hadil66/projects/4/views/1)

### Dinsdag 3 september

#### Sveltekit opzetten

#### create-svelte

Everything you need to build a Svelte project, powered by [create-svelte](https://github.com/sveltejs/kit/tree/main/packages/create-svelte).

#### Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```sh
npm create svelte@latest
npm create svelte@latest my-app
```

#### Developing

Once you've created a project and installed dependencies with **npm install** (or **yarn**), start a development server:

```sh
npm run dev
npm run dev -- --open  # Open in browser
```

#### Code conventies

- **Inspringen:** Na elk code-element inspringen voor duidelijkheid.
- **Comments:** Comments toevoegen om de code te verduidelijken, vooral in JavaScript en waar nodig in CSS.
- **CSS-structuur:** Generieke CSS plaats ik bovenaan.
- **Naamgeving:** Gebruik maken van '-' tussen woorden in.

### Woensdag 4 september

#### Sveltekit

Sveltekit is een library geschreven in Svelte (geoptimaliseerde HTML, CSS, JS gecombineerd) gemaakt voor het ontwikkelen van websites (snel en overzichtelijk websites).

**Belangrijke concepten:**

- SSR, SPA, MPA, SSG, meta framework → (svelte)kit
- PE → form: enhanced is true
- Folder-based routing
- GET en POST requests worden ‘onder water’ afgehandeld
- Elke route heeft een server component (view) bestand
- Data wordt geëxporteerd van het server bestand naar het Svelte component

**Error oplossen:**

```js
export let csr = false
```

### Donderdag 5 september

#### Basic design en profile card gebouwd

![Profile card voorbeeld](https://github.com/user-attachments/assets/d4f8040b-762e-4ddf-a700-c8b995fafb9d)

### Vrijdag 6 september

Feedback ontvangen squadpage zie [hier](https://github.com/Hadil66/your-tribe-for-life-squad-page/issues/7) en [hier](https://github.com/Hadil66/your-tribe-for-life-squad-page/issues/3). Vervolgens nieuwe [plannen gemaakt](https://github.com/Hadil66/your-tribe-for-life-squad-page/issues/8).

Ook heb ik feedback gegeven aan eerstejaars:

- [Issue 1](https://github.com/rutgerkock/your-tribe-for-life-squad-page/issues/18)
- [Issue 2](https://github.com/reyrey-https/your-tribe-for-life-squad-page/issues/19)
- [Issue 3](https://github.com/franceyourtribe/issues/5)
- [Issue 4](https://github.com/yrttribe/issues/20)

## Week 2

### Maandag 8 september

Componenten hergebruiken helpt om consistent en efficiënt te ontwerpen. Als een component op een plek wordt aangepast, wordt het overal aangepast.

### Dinsdag 9 september

Ik wilde vanilla JavaScript in mijn Svelte-project gebruiken, maar kreeg een internal error. Ik besefte dat de JavaScript op een andere manier geschreven moest worden. Op [Medium](https://medium.com/@edwinchiamaka2001/a-guide-to-dom-manipulation-in-sveltekit-2db08ccfbb39) las ik over de juiste methoden hiervoor. De `onMount`-functie zou gebruikt moeten worden.

### Woensdag 10 september

#### Creative coding with SvelteKit

**Progressive enhancement** is een strategie in webdesign die webinhoud centraal stelt. Het maakt basisfunctionaliteit toegankelijk voor iedereen, terwijl gebruikers met moderne browsers een verbeterde versie krijgen.

#### Stappenplan

1. Maak een tijdelijke kopie van de folder van de squadpage repo.
2. Installeer een schone installatie van SvelteKit voor de squadpage.
3. Voeg in `/routes/+page.js` deze regel code toe: `export let csr = false` *(dit kan je aanpassen)*.
4. Kopieer de code uit `/lib/fetch-node.js` van je laatste Node.js-project van sprint 12.
5. Importeer deze functie in `/routes/+page.server.js`.
6. Controleer of alles correct is geïmplementeerd aan de hand van het voorbeeld.
7. Copy-paste de toegevoegde Svelte-code terug in `/route/+page.svelte`.

## Week 3

### Maandag 16 september

#### Epics en Stories

Epics zijn een handige manier om werk te organiseren en een hiërarchie te creëren. Het idee is om werk op te splitsen in opleverbare stukken, zodat grote projecten kunnen worden afgerond en klanten op regelmatige basis waarde krijgen.

Structuur: **Epic → Stories → User Stories → Taken**

#### MoSCoW Prioriteringsmodel

- **Must have:** Dit moet af zijn op de deadline.
- **Should have:** Dit zou af moeten zijn, anders is het project incompleet.
- **Could have:** Dit kan worden toegevoegd als er tijd over is.
- **Won't have:** Goede ideeën die geen prioriteit hebben.

#### Planning Poker Workshop

Tijdens de **Planning Poker** workshop hebben we als team alle taken een numerieke waarde toegekend, gebaseerd op hun moeilijkheidsgraad en geschatte duur.

### Dinsdag 17 september

Vandaag heb ik een nieuw [profile card](https://your-tribe-for-life-profile-card-xi.vercel.app/) design gemaakt en gebouwd.

![Profile card design voorbeeld](https://prod-files-secure.s3.us-west-2.amazonaws.com/4d2d2910-0f35-4885-8674-f6228a3ebfa0/79051f99-1437-49db-b9d2-9f8394601c28/368479211-96cbc06e-988b-4eaf-81e0-2753b09a1a9f.png)

### Woensdag 18 september

De achtergrondafbeelding was niet zichtbaar. Dit heb ik opgelost door mijn styling naar de static map te verplaatsen. Zie de details in deze [commit](https://github.com/Hadil66/your-tribe-for-life-profile-card/commit/88085de111a7d8ce19aebd65cad340e79e5c21da).

#### Code Refactoring

**Code refactoring:** Het herschrijven van code volgens best practices zoals duidelijke conventies, goede semantiek, het verwijderen van commented code, geen overbodige `console.log()` statements en correcte tabs.

---

Dit document kan verder worden uitgebreid voor latere sprints!
