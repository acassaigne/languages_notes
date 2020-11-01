# Typescript 

## setup typescript language

download and setup:
https://www.typescriptlang.org/download


```bash
npm install typescript --save-dev
```

## Yarn

Package Manager & project manager

setup yarn 

```bash
npm install -g yarn
```

Better manage packages: `yarn`

for running tests:

```bash
yarn test
```

## setup js linter 

setup eslint 

```bash 
npm install -g eslint
```

## declare setter 

You have to use keyword `get` before a method name.


```typescript

    private readonly size: number;

    constructor(size: number) {
        this.size = size
    }

    get squareOfSum(): number {
        let result = 0;
        for (let i = 1; i <= this.size; i++) {
            result += i ;
        }
        return result * result;
    }

}

export default Squares
```