# 7DaysOfCode.Day05
7DaysOfCode.Day05

let frutas = [];
let laticinios = [];
let doces = [];
let congelados = [];
let comida = [];
let naoperecivel = [];
let acougue = [];
let categoria = ""; 

let adicionar = "sim"; 
while(adicionar != "nao"){
    adicionar = prompt("Gostaria de adicionar algum item a sua lista de compras ? || Responda 'sim' ou 'nao'");
    while (adicionar != "sim" && adicionar != "nao"){
       alert("Operação Inválida");
       adicionar = prompt("Gostaria de adicionar algum item a sua lista de compras ? || Responda 'sim' ou 'nao'"); 
    }

    if (adicionar === "nao") {
        break;
    }

    comida = prompt("Qual alimentos gostaria de adicionar ?");
    categoria = prompt("Qual a categoria do alimento ? 'frutas', 'laticinios', 'doces', 'Não perecível', 'Açougue' ou 'congelados'");
    if(categoria === 'frutas'){
        frutas.push(comida);
    } else if (categoria === 'laticinios'){
        laticinios.push(comida);
    } else if (categoria === 'doces'){
        doces.push(comida);
    } else if (categoria === 'congelados'){
        congelados.push(comida);  
    } else if (categoria === 'naoperecivel'){
        naoperecivel.push(comida);
    } else if (categoria === 'acougue'){
        acougue.push(comida);
    }    else {
        alert("Categoria não Definida!");
    }
}
alert(`Lista de compras:\n  Frutas: ${frutas}\n  Laticínios: ${laticinios}\n  Doces: ${doces}\n  Congelados: ${congelados}\n Não Perecível: ${naoperecivel}\n Açougue: ${acougue}`);
