Sujith M U
9037277948

Iam a UI developer working with pointcross lifesciences bangalore. Have total experience of 4 years working with javascript and javascript frameworks.
Yes i own a pc.
My personal working environment is built inside a linux system, with netbeans , sublime editor / notepad plus for coding.

https://stackoverflow.com/users/4705848/sujith-m-u
https://in.linkedin.com/pub/sujith-mu/2b/2a0/1a6

Iam interested in working with javascript and javascript frameworks along with libraries.

Coding
2) Write a function that takes a number and returns a list of its digits in an array.
/*
* @numbers
* Print each digit inside a number
*/
function numbers(num) {
	console.log((""+num).split(""));
}
var aNumber = 123456;
numbers(aNumber);

/*
* @unique
* returns unique items in an array
*/
3) Remove duplicates of an array and returning an array of only unique elements
function unique(arr) {
	var newArray = [];
	for(var i = 0;i < arr.length;i++) {
		if(newArray.indexOf(arr[i]) === -1) {
			newArray.push(arr[i]);
		}
	}
	console.log(newArray);
}
var newArr = [1,2,1,5,6,5];
unique(newArr);

/*
* implements Pig Latin
*/
4) Write function that translates a text to Pig Latin and back. English is translated to Pig Latin by taking the first letter of every word, moving it to the end of the word and adding ‘ay’. “The quick brown fox” becomes “Hetay uickqay rownbay oxfay”.
var orgText = "iam sujith mu",
    splitTxt = orgText.split(" "),
    finalOutput = "",
    slicedTxt = "";
for(var i = 0;i < splitTxt.length;i++) {
	var splitword = splitTxt[i].split("");
	for(var j = 0;j < splitword.length;j++) {
		slicedTxt = splitTxt[i].slice(1);
	}
	finalOutput += " "+slicedTxt+splitword[0]+"ay";
}
console.log(finalOutput.slice(1));

/*
* @rotate
* roatate an array with the specified number of positions
*/
5) Write a function that rotates a list by k elements. For example [1,2,3,4,5,6] rotated by 2 becomes [3,4,5,6,1,2]. Try solving this without creating a copy of the list. How many swap or move operations do you need?
var rotarr = [];
function rotate(arr, count) {
	for(var i = 0;i < count;i++) {
		rotarr.push(arr[i]);
	}
	var anoarr = arr.splice(count);
	console.log(anoarr.concat(rotarr));
}
rotate([1,2,3,4,5,6],4);
