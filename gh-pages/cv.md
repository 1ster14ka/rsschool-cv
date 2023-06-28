# Viktor Ivanov
### Novice developer

---

### Contact information:

**Phone:** +48 731 116 342<br>
**E-mail:** danyazybastik@gmail.com<br>
**Telegram:** @excusemebr00<br>

---

### Briefly About Myself:

I am 22 years old, **ambitious**, **fast**, with **character**. <br>
I studied as an assistant driver after working for half a year, I realized that this job was not for me.<br>
I prefer to puzzle over complex problems, well, I really like to solve complex problems, and when I solve them, <br> I feel such joy in my soul. Therefore, I really want to become a programmer and constantly develop in this area. <br>

---

### Skills and Proficiency:

Studied on my own *HTML*, *CSS*, *JavaScript*. Didn't get to frameworks.

---

### My code

 Battle Ship
```javascript
let min = 0;
let max = 8;
let rand = min + Math.random() * (max - min);
let random = Math.floor(rand);
let location1 = random;
let location2;
let location3;


if(location1 == 0){
  location2 = location1 + 1;
  location3 = location2 + 1;
}else if(location1 == 7) {
  location2 = location1 - 1;
  location3 = location2 - 1;
}else{
  location2 = location1 + 1;
  location3 = location1 - 1;
}


let hits = 0;
let guesses = 0;
let guess;
let isSank = false;

while(isSank == false) {
  guess = prompt('Enter num 0 - 7');
  if(guess < '0' || guess > '8') {
    alert('Enter valid num');
  }else{
    guesses += 1;
   if(guess == location1 || guess == location2 || guess == location3) {
      hits += 1;
      alert('Hits');
      if(guess == location1) {
        location1 = undefined;
      }else if(guess == location2) {
        location2 = undefined;
      }else if(guess == location3) {
        location3 = undefined;
      }
      if(hits == 3){
        isSank = true;
        alert(`Вы выстрелили ${guesses} и ваша точность ${3/guesses.toFixed(2)}`);
      }
    }else {
      alert('Miss');
    }
  }
};
```

---

### Languages:

- Ukrainian
- Russian
- English