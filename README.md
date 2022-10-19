# hacker-rank-10DaysOfJavascript-solutions
This repo contains the solutions for hacker rank 10 Days of Javascript challenge, which I completed in October,2022 <br> <br> <br>



Day-2 (javascript loops) :
function vowelsAndConsonants(s) {
 //Create Array of vowels
    const vowels = ["a","e","i","o","u"];
 //Convert String to Array
    const arr = s.split("");
 //Empty vowels and cons array
    var vowelsFound = [];
    var cons = [];
 //Push vowels and cons to their arrays
 for (let i = 0; i <= arr.length; i++) {
      if (vowels.includes(arr[i])) {
         vowelsFound.push(arr[i]);
         } else {
             cons.push(arr[i]);
         }
    }
 //ConsoleLog so that they in order and cons follows vowels on new lines
    console.log(vowelsFound.join('\n') + '\n' + cons.join('\n'))
 }
 //Test, Exclude in copy
 vowelsAndConsonants("javascriptloops"); 
