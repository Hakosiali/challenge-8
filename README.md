# challenge-8

//number 1
function filterEvenNumbers(arr) {
  return arr.filter(number => number % 2 === 0);
}
const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const evenNumbers = filterEvenNumbers(numbers);

console.log(evenNumbers);

//number 2
const abdelhak = { name: 'Abdelhak', age: 35, email: 'abdelhak@example.com' };
const mohamed = { name: 'Mohamed', age: 28, email: 'mohamed@example.com' };
const luffy = { name: 'Luffy', age: 40, email: 'luffy@example.com' };

const people = [abdelhak, mohamed, luffy];

function filterPeopleOver30(peopleArray) {
  return peopleArray.filter(person => person.age > 30);
}

const peopleOver30 = filterPeopleOver30(people);

console.log(peopleOver30);



//number 3
class Stack {
  constructor() {
    this.items = [];
  }

  push(element) {
    this.items.push(element);
  }

  pop() {
    if (this.isEmpty()) {
      return "Underflow";
    }
    return this.items.pop();
  }

  peek() {
    return this.items[this.items.length - 1];
  }

  isEmpty() {
    return this.items.length === 0;
  }

  size() {
    return this.items.length;
  }
}

const stack = new Stack();

stack.push(10);
stack.push(20);
stack.push(30);

console.log(stack.peek());
console.log(stack.pop()); 
console.log(stack.pop()); 

console.log(stack.isEmpty()); 
console.log(stack.size());    



// number 5
function removeVowels(inputString) {
  return inputString.replace(/[aeiouAEIOU]/g, '');
}

const originalString = "SAY MY NAME WALTER WHITE!";
const stringWithoutVowels = removeVowels(originalString);

console.log(stringWithoutVowels);


// number 6
function mergeAndRemoveDuplicates(arr1, arr2) {
  const mergedArray = arr1.concat(arr2);
  return Array.from(new Set(mergedArray));
}

const array1 = [1, 2, 3, 4];
const array2 = [3, 4, 5, 6];

const uniqueMergedArray = mergeAndRemoveDuplicates(array1, array2);

console.log(uniqueMergedArray);
