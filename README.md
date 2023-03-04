# PRG04-2022-2023

## 👾👾👾 Object oriented game development 👾👾👾

In dit vak gaan we games bouwen met [excalibur](https://excaliburjs.com) in een moderne web development omgeving.

We leren Object Oriented Programming (OOP) omdat je dit in je carriere als developer veel zal tegenkomen en omdat het erg goed werkt voor het bouwen van games.

<br>
<Br>

### Excalibur

[Excalibur](https://excaliburjs.com) is een object-oriented library is die gebruik maakt van typescript. Excalibur geeft je een makkelijke manier om te werken met:

- Collision detection
- Physics
- Animaties
- Besturing

### Professioneel web development

Je leert de setup van een modern web development project met behulp van [Parcel](https://parceljs.org) en [Typescript](https://www.typescriptlang.org). Dit is niet alleen van toepassing voor games maar eigenlijk voor elk front-end web development project.

<br>
<br>
<br>

## Onderwerpen

| Les | OOP Theorie ochtend | Game Theorie middag | 
|------|---------|----------|
| 1 | Classes en instances. Class diagram. | Werkomgeving met Excalibur. Endless runner. | 
| 2 | Composition en Encapsulation | Shark en array van Fishes. Vector en collision. Spawning and removing objects. | 
| 3 | Composition en Encapsulation | Spawning en removing. Object pool. Physics toevoegen. |
| 4 | Inheritance | Excalibur classes extenden, eigen classes extenden. |
| 6 | Typescript tips en truuks | [Game op Arcade Kast plaatsen](https://github.com/HR-CMGT/PRG04-2021-2022-controller) | 
| 7 | Game development | Verschillende game mechanics en systems |
| 8 | Game development | Vraaggestuurd | 



<br>
<br>
<br>

## Excalibur Basics

- [Excalibur JS](https://excaliburjs.com)
- [Actors](https://excaliburjs.com/docs/actors)
- [Sprites](https://excaliburjs.com/docs/sprites)
- [Physics](https://excaliburjs.com/docs/physics)

## Startcode

- [Voorbeeld project 1: leeg startproject]()
- [Voorbeeld project 2: Sprites laden, animeren en collisions]()
- [Voorbeeld project 3: Physics toepassen]()

<br>
<br>
<br>

## OOP Basics

Een typescript class schrijf je als volgt.

```typescript
class Fish {
    private score = 10
    constructor() {
        console.log("I'm a fish")
    }
    showScore(){
        console.log(this.score)
    }
}
```

Door een excalibur class te extenden kan je je eigen functionaliteit toevoegen.

```typescript
import { Actor, Vector } from 'excalibur'
class Fish extends Actor {
    private score = 10
    constructor() {
        this.pos = new Vector(100,100)
        this.vel = new Vector(20,20)
    }
}
```

<br>
<br>
<br>

## Parcel Basics

Je ontwikkelt in de `src` folder. Door in de terminal `npm  start` te typen start je de development server. Als je project af is typ je `npm build`. Je project komt automatisch terecht in de `docs` folder. In github pages kan je vervolgens aangeven dat je `docs` folder live moet staan.

<br>
<br>
<br>

## Links

- [Typescript](https://www.typescriptlang.org)
- [MDN Game Development](https://developer.mozilla.org/en-US/docs/Games)
- [Voortgang opslaan met localStorage](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage)
- [Online Multiplayer met Socket.IO](https://socket.io) of [Lance](https://lance-gg.github.io)
- [Create Game Sounds](https://sfxr.me)
- [Genereer je Class Diagram met markdown](https://mermaid-js.github.io/mermaid-live-editor/edit#pako:eNp9ks1uwyAMgF8F-bStzQtEO037uewwqVcuTvBatPAjA1Kjru--pBSUZto4IPRhPhvDCXqnCFroBwzhWeOe0UgrrZjGGxoSD00jnlLXDbSCrzocSuTOs44kHr8rX9OiyDuXbFl1ymQeG5tMRyxC75gW-EMftfDTtGDJK4x0d79Ayll6d6i03Rd-vk2Yi6gZm5LPE6kCf5k3fnD-D-F81_91za1udT53qBpKA45rMFagKER2Y_XBFgyxQa2mR7yIJMQDGZLQTkuF_CVB2jkuV_KidHQM7ScOgbaAKbrdaHtoIycqQdePcI06_wCsKKak)