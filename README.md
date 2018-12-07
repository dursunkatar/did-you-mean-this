# csharp-js-did-you-mean-this

Bunumu demek istediniz ?

Yazılan yanlış kelimeyi,kelime dizisindeki diğer kelimelerle karşılaştırarak yanlış kelimeye en çok benzeyeneni bulup doğru kelimeyi tespit eder

### C sharp Örnek
```csharp
string[] words = { "google","kedi", "kobra" };

var corrector = new DidYouMeanThis
{
    Words = words
};

Console.WriteLine(corrector.IsThis("gogıl"));
// google
Console.WriteLine(corrector.IsThis("kdi"));
// kedi
Console.WriteLine(corrector.IsThis("kbr"));
// kobra
```

### javascript Örnek

```js
let words = ["google", "kedi", "kobra"];

let corrector = new DidYouMeanThis(words);

console.log(corrector.isThis("gogıl"))
// google
console.log(corrector.isThis("kdi"))
// kedi
console.log(corrector.isThis("kbr"))
// kobra
```
