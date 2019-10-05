# TypeScript

## INTERFACE

#### un exemple dans lequel on utilise 2 interfaces

```
interface Books {
    title: string;
}

interface Author {
    name: string;
    firstname: string;
    collection: Books[]
}


function getMessage (author: Author): string {
    const message = `${author.name} ${author.firstname} possède ${author.collection.length} livres`;
    return message;
}

const books1 = [{ title: 'livre1' }, { title: 'livre3' }];

const author1 = {
  name: 'Dupond',
  firstname: 'Jean',
  collection: books1
}

const msg = getMessage(author1);

console.log(msg);
```

> **Note:** le retour sera *Dupond Jean possède 2 livres*

