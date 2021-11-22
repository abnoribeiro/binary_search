# binary_search
Example binary search in javascript

{
var list = [1, 3, 5, 7, 9, 15];

const binary_search = (list, item) => {
    var low = 0;
    var high = list.length - 1;

    while(low <= high){
        var middle = Math.floor((low + high) / 2);
        var guess =   list[middle];

        if(guess == item){
            return middle
        }
        if(guess > item){
            high = middle - 1; 
        }
        else{
            low = middle + 1;
        }
    }
    return "None"     
}
}
