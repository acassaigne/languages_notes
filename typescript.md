# Typescript 

## setup typescript language

download and setup:
https://www.typescriptlang.org/download


```bash
npm init
npm install --save-dev typescript tslint @types/node 
```

## config `tsconfig.json`


https://stackoverflow.com/questions/61305578/what-typescript-configuration-produces-output-closest-to-node-js-14-capabilities

```json
{
    "compilerOptions": {
        "lib": ["es2020"],
        "module": "commonjs",
        "moduleResolution": "node",
        "sourceMap": true,
        "outDir": "dist",
        "strict": true,
        "target": "es2020",
    },
    "include": [
        "src"
    ]
}
```

## configure tsling

```bash
./node_modules/.bin/tslint --init
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