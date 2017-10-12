# win-paperclip

Make more paperclips

http://www.decisionproblem.com/paperclips

```js
// --- paste into console

function click (id) {
  document.querySelector(id).click();
}

function multiClick (id, n) {
  for (i = 0; i < n; i++) {
    click(id);
   }
}

function delayedClick (id, delay) {
  setTimeout(function () { click(id); }, delay);
}

function timeClick (id, delay, nTimes) {
  for (i = 0; i < nTimes; i++) {
    delayedClick(id, i * delay);
  }
}

var bMakePaperclip = '#btnMakePaperclip',
    bAutoClipper = '#btnMakeClipper',
    bWire = '#btnBuyWire',
    bMarketing = '#btnExpandMarketing',
    bProcessors = '#btnAddProc',
    bMemory = '#btnAddMem',
    bRaise = '#btnRaisePrice',
    bCompute = '#btnQcompute',
    bMegaClippers = '#btnMakeMegaClipper';

// --- end paste

// examples:
multiClick(bMakePaperClip, 100)
timeClick(bAutoClipper, 15000, 25)
timeClick(bProcessors, 120000, 20)
timeClick(bMemory, 120000, 20)
timeClick(bMarketing, 500000, 20)
    
// cheats
wire = 9999999
investUpgrade()

```
