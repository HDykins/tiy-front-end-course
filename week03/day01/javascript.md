2.
function validateParameter(input) {
if (typeof input === "string" && input.length>0){
return true;
} else {
return false; 
}
}

validateParameter();

3.
function findInList(word, character) {
word = word.toLowerCase();
var sum = 0
if (typeof word === "string" && typeof character === "string") {
for (var counter=0; counter<word.length; counter=counter+1) {
if (character===word[counter]) {
sum = sum + 1
}
}
}
return sum;
}

findInList();

4.
function squareList(array) {
var SQ=[];
if (typeof array === "object") {
for (var counter=0; counter<array.length; counter=counter+1) {

SQ.push(array[counter]*array[counter]);
}
}
return SQ;
}

squareList();

5.
function filterList(array) {
var filter=[];
if (typeof array === "object") {
for (var counter=0; counter<array.length; counter=counter+1) {
if (typeof array[counter] === "string") {
filter.push(array[counter]);
}
}
}
return filter;
}

filterList();

6.
function iterateList(myArray,myFunction) {
for (counter=0; counter<array.length; counter = counter + 1) {
myFunction(myArray[counter];
}                
}

iterateList([1, 2, 3, 4, 5], function (listItem) {
console.log(listItem);
});

7.
function add(number1) {
return function (number2) {
return (number1 + number2);
};
}

var add5 = add(5);
var sum = add5(10);

console.log(sum);

8.
var message = (function () {
var message = 'Welcome';

function getMessage() {
return message;
}

return {
getMessage: getMessage
};
})();

console.log(message.getMessage());


9.
function mergeArrays(array1,array2) {

var newArray =[];
for(var counter=0; counter<array1.length; counter=counter+1) {
newArray.push([array1[counter],array2[counter]]);
}

return newArray;
}


mergeArrays([1,2,3], ["a","b","c"]);