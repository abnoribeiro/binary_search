# binary_search
Example binary search in javascript

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

binary_search(list, 1)

❶ baixo e alto acompanham a parte da lista que você está procurando.
❷ Enquanto ainda não conseguiu chegar a um único elemento...
❸ … verica o elemento central.
❹ Acha o item.
❺ O chute foi muito alto.
❻ O chute foi muito baixo.
❼ O item não existe.
❽ Vamos testá-lo!
❾ Lembre-se, as listas começam no 0. O próximo endereço tem índice 1.
❿ “None” signica nulo em Python. Ele indica que o item não foi encontrado.
