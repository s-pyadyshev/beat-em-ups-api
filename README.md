Beat'em Ups API

<b>Examples</b>
<br/>
<br/>
Get all games info:<br/>
```javascript
fetch("https://raw.githubusercontent.com/s-pyadyshev/beat-em-ups-api/master/db.json")
  .then(result => result.json())
  .then(data => data);
```

Get all games names:<br/>
```javascript
fetch("https://raw.githubusercontent.com/s-pyadyshev/beat-em-ups-api/master/db.json")
  .then(result => result.json())
  .then(data => data.map(game => game.name));
```

Get all games with 4 players:<br/>
```javascript
fetch("https://raw.githubusercontent.com/s-pyadyshev/beat-em-ups-api/master/db.json")
  .then(result => result.json())
  .then(data => data.filter(game => game.players === 4));
```