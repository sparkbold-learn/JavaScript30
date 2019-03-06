## Key take away

- use attribute selector
  `audio = document.querySelector(`audio[data-key="${e.keyCode}"]`)`

- check the null case `if (!audio) return`

- rewind audio file before playing

- add new class in vanilaJS `key.classList.add('playing')`

- clear transition at the end of transition `transitionend` event: `keys.forEach(key => key.addEventListener('transitionend', removeTransition))`

- in removeTransition function skip the function if it is not transform `if (e.propertyName !== 'transform') return;`
