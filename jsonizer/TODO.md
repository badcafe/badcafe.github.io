# Enhancement

```typescript
    // subrevivers
} & Target extends Array<infer Item>
? {
    [index: number]: Reviver<Item>
}
: {
    [key in keyof Target]: Reviver<Target[key]>
};
```

=========

Submappers :

Quand on extrait un submapper:
* si l'objet obtenu est une classe, ok
* sinon, il doit pointer sur son parent, et si on a une chaîne vers une classe ancêtre, le submapper devrait être stringifié en fonction :

```
'org.acme.Person[hobbies][0]'
```

on devrait pouvoir retrouver la classe Person dans le registre, obtenir son reviver et son submapper, puis son submapper
