# make-right.github.io
Lets make things right

# Blog
## Javascript Code to add commas and quote
### Add commas using general for loop
```js
   // for loop version to format to 72 characters
for(let i=0,opArrIdx = 0;i<inputArray.length;i++){
    if(outputArray.length > 0 && inputArray[i]){
        let currLen = outputArray[opArrIdx].length; 
        let newLen = currLen + inputArray[i].length;
        if(newLen > maxLength ){
            opArrIdx++
        }
    }
    if(outputArray[opArrIdx]){
        outputArray[opArrIdx] = outputArray[opArrIdx] + inputArray[i];
    }
    else{
        outputArray[opArrIdx] = inputArray[i];
    }
}
```