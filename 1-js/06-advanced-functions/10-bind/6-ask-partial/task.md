importance: 5

---

# Giriş işlemi için kısmi uygulama.

Bir önceki <info:task/question-use-bind>'dan biraz daha karmaşık bir göreviniz var.

`user` objesi değiştirildi. Şimdi `loginOk/loginFail` fonksiyonlarının yerine tek bir fonksiyon `user.login(true/false)` var.

<<<<<<< HEAD:1-js/06-advanced-functions/11-currying-partials/1-ask-currying/task.md
Aşağıdaki `askPassword`'a ne iletilirse bu `user.login(true)`'u `ok` veya `user.login(fail)`'i `fail` olarak çağırır?
=======
What should we pass `askPassword` in the code below, so that it calls `user.login(true)` as `ok` and `user.login(false)` as `fail`?
>>>>>>> dccca58f268ad6d5a6f2160613a8ea3c5cd53a2d:1-js/06-advanced-functions/10-bind/6-ask-partial/task.md

```js
function askPassword(ok, fail) {
  let password = prompt("Password?", '');
  if (password == "rockstar") ok();
  else fail();
}

let user = {
  name: 'John',

  login(result) {
    alert( this.name + (result ? ' logged in' : ' failed to log in') );
  }
};

*!*
askPassword(?, ?); // ?
*/!*
```
Sadece işaretlenmiş bölümde gerçekleştiriniz.