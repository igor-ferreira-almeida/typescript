
# Preparando o ambiente

Atualização do npm
```
npm i -g npm-upgrade
```


Criar o package.json
```
npm init
```

Para instalar o TypeScript 
```
npm install typescript@VERSÃO --save-dev
```

Criar o arquivo tsconfig.json na raiz do projeto (na mesma pasta de package.json)

Conteúdo:
```
{
    "compilerOptions": {
        "target": "es6", //código traduzido
        "outDir": "js" //compilados
    },
    "include": [
        "ts/**/*" //source
    ]
}
```

adicionar no arquivo package.json um novo script

```
"compile": "tsc"
```

```
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "compile": "tsc"
},
```


Após isso executar o comando:
```
npm run compile
```

Para que o arquivo .js não seja gerado com erros de compilação é necessário colocar uma nova propriedade em tsconfig.json

