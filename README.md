# What-I-Learned-week-8

### All About That Text

* Event listener functions.
* Reading strings from input boxes.
* String building and manipulation.
* Keeping our back end and front end separate.
* Function expressions.
* Creating, appending, and removing elements.

#** Example **#
const result = document.querySelector('.result')
function printValue(text) {
    let newLi = document.createElement("LI");
    let textNode = document.createTextNode(text);
    newLi.appendChild(textNode);
    result.appendChild(newLi);
}
// const lis = document.querySelectorAll('ul li')
function clearResult(){
    const lis = document.querySelectorAll('ul li')
    for (const li of lis) {
        li.remove();
    }
}


# Just How We Roll

* Every time we click on a die, we get back a random result according to the possibilities of that die or set of dice.
* Change the DOM based only on simple input, not the state of anything on the DOM.


#** Example **#

const d6roll  = function(){

let num = getRandomNumber(6)
console.log(num)
sixes.push(num)

d6.src = `images/d6/${num}.png`;

let d6MedianNUM = median(sixes)

const d6Median = document.querySelector('#d6-rolls-median')
d6Median.innerText = d6MedianNUM;

let d6MeanNUm = mean(sixes)

const d6mean = document.querySelector('#d6-rolls-median')
d6mean.innerText = d6MeanNUm;

}
