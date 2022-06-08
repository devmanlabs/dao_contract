`/contracts/` is organized as follows:

- `/contracts/schemes/`- contracts necessary for PrimeDAO functioning on DAOStack.
- `/contracts/incentives/`- contracts that enable PrimeDAO users to create new yield farming programs.
- `/contracts/seed/`- Prime Launch seed module contracts.
- `/contracts/utils/`- utility contracts.

## Development

requires 

```
node >= 12.16.2
npm >= 7.8.0
````

to install node modules

```
npm i
```

to compile run
```
npm run compile
```

to test
```
npm run test
```

to run coverage
```
npm run coverage
```

### Deploy DAO to kovan

prepare `.env` file and add your config variables, it should look as follows:
```
NETWORK=kovan
PROVIDER=https://kovan.infura.io/v3/your-infura-provider-key
KEY=your-private-key
```

deploy external contracts
```
npm run deploy:contracts:kovan
```

deploy dao
```
npm run deploy:dao:kovan
```

### Setup deployed contracts on kovan

create configurable rights pool
```
npm run create:pool:kovan
```

initialize staking rewards contract  
```
npm run init:staking:kovan
```

## License
```

Licensed under the GNU General Public License v3.0.
You may obtain a copy of this license at:

https://www.gnu.org/licenses/gpl-3.0.en.html

```
