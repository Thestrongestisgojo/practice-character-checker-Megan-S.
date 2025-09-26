# practice-character-checker-Megan-S.
// 1. Prompt the user for a word or phrase
let userInput = readlineSync.question("Enter a word or phrase: ");

// 2. Prompt the user for an index number
let indexInput = readlineSync.question("Enter the index of the character you want to see: ");

// Convert the index to a number
let index = Number(indexInput);

// 3. Access the character using bracket notation
let character = userInput[index];

// 4. Print out the character
if (character !== undefined) {
    console.log(`The character at index ${index} is: '${character}'`);
} else {
    console.log(`Invalid index. Please enter a number between 0 and ${userInput.length - 1}.`);
