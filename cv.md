## [rsschool-cv](rsccool-cv)


# Chaikin Sergey

# My Contact Info

* **Address:** Russia, city of Astrakhan
* **Phone:** +7 937 137 05 06
* **E-mail:** [chaikin.sergey@gmail.com](chaikin.sergey@gmail.com)
* **LinkedIn:** [Sergey Chaikin](https://www.linkedin.com/in/sergey-chaikin-66730487/)
* **GitHub:** [voidstone](https://github.com/voidstone)
* **Codewars:** [voidstone](https://www.codewars.com/users/voidstone)
* **HackerRank:** [cyberzomby](https://www.hackerrank.com/cyberzomby)
* **Freecodecamp:** [serzh](https://www.freecodecamp.org/serzh)

# Summary
If I am good, then I am good; if I am bad, what is the point in denying it?
I do things others can't or don't know how to do.
if a guy like me wants to be respected, he has to be five times better than a regular programmer, and that guy has to do ten times as much. Otherwise, you may not wait for your chance.

# Skills

* Ubuntu,MacOs
* PHP, Javascript, SQL, Java and more (in passive state).
* MariaDB, MySQL, PostgreSQL


# Code examples

```js
var countChange = function(money, coins) {
  // your implementation here
  var count = 0;
  //var coins = [1, 2, 5, 10, 20, 50, 100, 200];

  var changer = function(index, value){

    var currentCoin = coins[index];

    if( index === 0){
      if( value % currentCoin === 0){
        count++;
      }
      return;
    }

    while( value >= 0 ){
      changer(index-1, value);
      value -= currentCoin;
    }
  }
  changer(coins.length-1, money);
  return count;
}
```