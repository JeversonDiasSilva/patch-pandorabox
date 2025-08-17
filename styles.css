const creditDisplay = document.getElementById('creditDisplay');
const addCreditBtn = document.getElementById('addCreditBtn');
const useCreditBtn = document.getElementById('useCreditBtn');
const coinSound = document.getElementById('coinSound');
const whatsappLink = document.getElementById('whatsappLink');
const clickSound = document.getElementById('clickSound');

let credits = 0;

function updateDisplay() {
  creditDisplay.textContent = credits;
}

function addCredit() {
  credits++;
  updateDisplay();
  coinSound.currentTime = 0;
  coinSound.play();
}

function useCredit() {
  if (credits > 0) {
    credits--;
    updateDisplay();
    clickSound.currentTime = 0;
    clickSound.play();
  } else {
    alert("Sem créditos disponíveis!");
  }
}

addCreditBtn.addEventListener('click', addCredit);
useCreditBtn.addEventListener('click', useCredit);

// Tocar som ao clicar no WhatsApp, antes de abrir
whatsappLink.addEventListener('click', function(e) {
  e.preventDefault();
  coinSound.currentTime = 0; // Som de crédito aqui
  coinSound.play();

  setTimeout(() => {
    window.open(this.href, '_blank', 'noopener');
  }, 400);
});
