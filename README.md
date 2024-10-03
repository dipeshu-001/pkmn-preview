# team-preview
Pokémon team preview image generator

## Install

Install pkmn-preview:
```
npm i pkmn-preview
```


### Generate a summary

```ts
import { Sets } from '@pkmn/sets';
import { summaryScreen, partyScreen } from 'team-preview';

//Pokémon Showdown! set
const set = Sets.importSet(
`Gekkouga (Greninja-Ash) (M) @ Choice Specs  
 Ability: Battle Bond  
 Level: 100  
 Shiny: Yes  
 Pokeball: Cherish Ball  
 EVs: 252 SpA / 4 SpD / 252 Spe
 Timid Nature
 - Hydro Pump
 - Dark Pulse
 - Water Shuriken
 - Spikes
`);

const buffer = await summaryScreen(set);
```

### Generate a party preview

```ts
import { summaryScreen, partyScreen } from 'team-preview';

//array of 6 sets
const buffer = await partyScreen([set, set2, set3, set4, set5, set6]);
```


### Credits

This project currently being owned and maintained by __dipeshu-001.__
