# GameAction/bananalotto

This repository created to play on bananalotto website and play grids

## 💻 Usage

Install the package as a dependency from [npm](https://www.npmjs.com/package/@game-action/bananalotto):

```bash
npm install --save-dev @game-action/bananalotto
```
or
```bash
yarn add -D @game-action/bananalotto
```

### TypeScript

```typescript
import { Bananalotto } from "@game-action/bananalotto";

// to connect
const king = await Bananalotto.init("email", "password");

// fetch summary information
const summary = await king.summary();
console.log(summary); // Summary { grid: 10, cash: 0.06, point: 6750 }

// play grid, max of 10 per day
const grid = await king.playGrid();
console.log(grid); // true or false
```

## 📄 License

- Code: [MIT](./LICENSE) © [Rémy BRUYERE](https://remy.ovh)

<p align="center">
  <sub>An open source project by <a href="https://remy.ovh">rem42</a></sub>
</p>
