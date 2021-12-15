# codigo_util

### Alternativa a if/elseif infitito o switch case
```
const objOpciones = {
  opcion1: 'Res1',
  opcion2: 'Res2',
  opcion3: 'Res3',
  opcion4: 'Res4',
};

respuesta = objOpciones['opcion1'];
console.log(respuesta); //R: Res1
```

### Crear y usar promesas
```
// crear promesa
function miFuncion (n1, n2) {
  return new Promise((resolve, reject) => {

    const resultado = n1 + n2;

    resolve(resultado);
    reject(new Error('Ha ocurrido un error'));

  });
}

// utilizar promesa
miFuncion(22, 88)
  .then(resolve => {
    console.log(resolve); // 110
  })
  .catch(error => { //reject
    console.log(error); // obj Error
  })
```
