# nCr
Combination nCr


let factorial = function(number){

    let fact = 1;
    for (let i = 1; i <= number; i++){
        fact = fact * i;
    }
    return fact
}

let combination = function(n, r){
    let factN = factorial(n);
    let factR = factorial(r);

    let nCr = factN / (factorial(n-r) * factR);

    return nCr;
}


console.log(combination(5, 3));
