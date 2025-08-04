//terror, comedia 

//The monkey
//Influência
//Beware the Slenderman
//A entidade
//Os Farofeiros 2

let campoIdade;
let campoComedia;
let campoTerror;

function setup() {
  createCanvas(800, 400);
  createElement("h2", "Recomendador de filmes");
  createSpan("Sua idade:");
  campoIdade = createInput("5");
  campoComedia = createCheckbox("Gosta de Comedia?");
  campoTerror = createCheckbox("Gosta de Terror?");
}

function draw() {
  background("white");
  let idade = campoIdade.value();
  let gostaDeComedia = campoComedia.checked();
  let gostaDeTerror = campoTerror.checked();
  let recomendacao = geraRecomendacao(idade, gostaDeComedia, gostaDeTerror);

  fill(color(76, 0, 115));
  textAlign(CENTER, CENTER);
  textSize(38);
  text(recomendacao, width / 2, height / 2);
}

function geraRecomendacao(idade, gostaDeTerror, gostaDeComedia) {
  if (idade >= 18) {
    if (idade >= 14) {
      return "The Monkey";
    } else {
      if (idade >= 12) {
        if(gostaDeComedia || gostaDeTerror) {
          return "Influência";          
        } else{
         return "Beware the Slenderman";
        }
      } else {
        if (gostaDeComedia) {
          return "A entidade";
        } else {
          return "Os Farofeiros";
        }
      }
    }
  } else {
    if (gostaDeComedia) {
      return "Beware the Slenderman";
    } else {
      return "Influência";
    }
  }
}
