```js
let user = {
  name: 'Arya',
  sibling: ['Robb', 'Ryan', 'John'],
};
let allBrothers = ['Robb', 'Ryan', 'John'];
let brothersCopy = user.sibling;
let usename = user.name;
let newUser = user;
```

1. Memory representation

- Create the memory representation of the above snippet on notebook.
- Take a photo/screenshot and add it to the folder `code`

<!-- To add this image here use ![name](./hello.jpg) -->

2. Answer the following with reason:

- `user == newUser;` // true, Both the objects are having the same reference number, so they both are equal.
- `user === newUser;` // true, Both the objects are having the same reference number, so they both are equal, typeof the reference number is number , so they are strictly equal.
- `user.name === newUser.name;` // true, Both the objects refers to the same reference number , so the content which they point through object.name is also strictly equal(both are number datatype value).
- `user.name == newUser.name;`// true, Both the objects refers to the same reference number , so the content which they point through object.name is also equal.
- `user.sibling == newUser.sibling;`// true, Both the objects refers to the same reference number , so the content which they point through object.sibiling is also equal.
- `user.sibling === newUser.sibling;`/ true, Both the objects refers to the same reference number , so the content which they point through object.sibiling is also strictly equal(both are number datatype value).
- `user.sibling == allBrothers;`//false , Because user.sibiling is the object with reference number, all theBrothers is an array stored by value, so they cant be equal.
- `user.sibling === allBrothers;`//false , Because user.sibiling is the object with reference number, all theBrothers is an array stored by value, so they cant be equal.so it will not be strictly equal anyways.
- `brothersCopy === allBrothers;`//false , Because "brotherCopy" = "user.sibiling" is the object with reference number, all theBrothers is an array stored by value, so they cant be equal.so it will not be strictly equal anyways.
- `brothersCopy == allBrothers;`//false , Because "brotherCopy" = "user.sibiling" is the object with reference number, all theBrothers is an array stored by value, so they cant be equal.
- `brothersCopy == user.sibling;`// true, Both the objects refers to the same reference number , so the content which they point through object.sibiling is also equal.
- `brothersCopy === user.sibling;`// true, Both the objects refers to the same reference number , so the content which they point through object.sibiling is also equal.they are of same type, so they are strictly equal.
- `brothersCopy[0] === user.sibling[0];`// true, Both the objects refers to the same reference number , so the content which they point through same object.sibiling and index is also equal.they are of same type, so they are strictly equal.
- `brothersCopy[1] === user.sibling[1];`// true, Both the objects refers to the same reference number , so the content which they point through same object.sibiling and index is also equal.they are of same type, so they are strictly equal.
- `user.sibling[1] === newUser.sibling[1];`// true, Both the objects refers to the same reference number , so the content which they point through same object.sibiling and index is also equal.they are of same type, so they are strictly equal.
