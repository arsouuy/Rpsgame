var totalscore = {
  playerscore: 0
};

// Function to get a random computer choice
function getComputerChoice() {
  const choices = ['Rock', 'Paper', 'Scissors'];
  let randomnum = Math.floor(Math.random() * 3);
  return choices[randomnum];
}

// Function to determine the result
function getResult(playerChoice, computerChoice) {
  let score = 0;  

  if (playerChoice === computerChoice) {
      score = 0;
  } else if (playerChoice === 'Rock' && computerChoice === 'Scissors') {
      score = 1;
  } else if (playerChoice === 'Paper' && computerChoice === 'Rock') {
      score = 1;
  } else if (playerChoice === 'Scissors' && computerChoice === 'Paper') {
      score = 1;
  } else {
      score = -1;
  }

  return score;
}


// Function to show the result
function showResult(score, playerChoice, computerChoice) {
  let result = document.getElementById('result');
  if (score === 1) {
      result.innerText = 'You Win!';
  } else if (score === -1) {
      result.innerText = 'You Lose!';
  } else {
      result.innerText = 'It\'s a Draw!';
  }

  let hands = document.getElementById('hands'); 
  hands.innerText = `Computer: ${computerChoice} vs You: ${playerChoice}`;
  
  let playersco = document.getElementById('player-score');
  playersco.innerText = `Score: ${totalscore['playerscore']}`;
}



// Function for handling player choice
function onClickRPS(playerChoice) {
  const computerChoice = getComputerChoice();
  const score = getResult(playerChoice, computerChoice);
  
  totalscore['playerscore'] += score;
  showResult(score, playerChoice, computerChoice);
}



// Function to set up button listeners
function playGame() {
  const rpsButtons = document.querySelectorAll('.rpsButton');
  rpsButtons.forEach(rpsButton => {
      rpsButton.onclick = () => onClickRPS(rpsButton.value);
  });
 let endbutton= document.getElementById('endGameButton')
 endbutton.onclick=()=>{endGame(totalscore)}
}





// Function to clear the game (optional, not yet implemented)
function endGame(totalscore) {
  
  totalscore=0

  const result = document.getElementById('result'); 
  const hands = document.getElementById('hands'); 
  const playersco = document.getElementById('player-score');

  
  result.innerText = ''; 
  hands.innerText = ''; 
  playersco.innerText = '';
  


  
}

// Start the game
playGame();
