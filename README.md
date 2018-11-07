# counting-cards
var count = 0;

function cc(card) {
  switch(card) {
    case 2:
    case 3:
    case 4:
    case 5:
    case 6:
    count = count + 1;
    break;
    case 10:
    case 'J':
    case 'Q':
    case 'K':
    case 'A':
    count = count - 1;
    break;
  } 
  //return count + (count > 0 ? " Bet" : " Hold");
  
  if (count > 0) {
    return count + " Bet";
  } else if (count <= 0) {
    return count + " Hold"
  }
}

// Add/remove calls to test your function.
// Note: Only the last will display
cc(10); cc('J'); cc('K'); cc('A'); cc(10);
console.log(count);// Only change code below this line
  
