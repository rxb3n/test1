<template>

  <img src="../src/assets/full.jpeg" alt="">

  <div class="eng">
    <h1>To English</h1>
    <div class="input">
      <input v-model="text" id="toenglish">
      <button class="btn" @click=translateAb()>Translate</button>
      <p>Translation : {{ outputAb }}</p>
    </div>

  </div>

  <div class="ang">
    <h1>To Angelish</h1>
    <div class="input">
      <input v-model="message" id="toang">
      <button class="btn" @click=translateBa()>Translate</button>
      <p>Translation : {{ outputBa }}</p>
    </div>
  </div>

</template>

<script>

export default {
  data() {
    return {
      outputAb: [],
      outputBa: [],
    }
  },

  methods: {
    translateAb() {
      let input = document.getElementById("toenglish").value;
      this.outputAb = [];

      for (let i = 0; i < input.length; i++) {
  
 
  if (input[i] == "1") {
    this.outputAb.push("q");
  }
  
      else if (input[i] == "2") {
        this.outputAb.push("w");
  }
  
      else if (input[i] == "3") {
        this.outputAb.push("e");
  }
  
          else if (input[i] == "4") {
            this.outputAb.push("r");
  }
  
          else if (input[i] == "5") {
            this.outputAb.push("t");
  }
  
          else if (input[i] == "6") {
            this.outputAb.push("z");
  }
  
          else if (input[i] == "7") {
            this.outputAb.push("u");
  }
  
          else if (input[i] == "8") {
            this.outputAb.push("i");
  }
  
          else if (input[i] == "9") {
            this.outputAb.push("o");
  }
  
          else if (input[i] == "0") {
            this.outputAb.push("p");
  }
  
              else if (input[i] == "@") {
                this.outputAb.push("a");
  }
  
              else if (input[i] == "#") {
                this.outputAb.push("s");
  }
  
              else if (input[i] == "$") {
                this.outputAb.push("d");
  }
  
              else if (input[i] == "_") {
                this.outputAb.push("f");
  }
  
              else if (input[i] == "&") {
                this.outputAb.push("g");
  }
  
              else if (input[i] == "-") {
                this.outputAb.push("h");
  }
  
              else if (input[i] == "+") {
                this.outputAb.push("j");
  }
  
              else if (input[i] == "(") {
                this.outputAb.push("k");
  }
  
              else if (input[i] == ")") {
                this.outputAb.push("l");
  }
  
                  else if (input[i] == "*") {
                    this.outputAb.push("y");
  }
  
                  else if (input[i] == '"') {
                    this.outputAb.push("x");
  }
  
                  else if (input[i] == "'") {
                    this.outputAb.push("c");
  }
  
                  else if (input[i] == ":") {
                    this.outputAb.push("v");
  }
  
                  else if (input[i] == ";") {
                    this.outputAb.push("b");
  }
  
                  else if (input[i] == "!") {
                    this.outputAb.push("n");
  }
  
                  else if (input[i] == "?") {
                    this.outputAb.push("m");
  }
  
                         else if (input[i] == " ") {
                          this.outputAb.push(" ");
  }

  
  
}
let outputJ = this.outputAb.join("");
this.outputAb = outputJ
console.log(outputJ);
return outputJ;


},

  translateBa() {
    let input = document.getElementById("toang").value;
      this.outputBa = [];

      for (let i = 0; i < input.length; i++) {
        if (input[i] == "q") {
          this.outputBa.push("1");
    }
    
        else if (input[i] == "w") {
          this.outputBa.push("2");
    }
    
        else if (input[i] == "e") {
          this.outputBa.push("3");
    }
    
            else if (input[i] == "r") {
              this.outputBa.push("4");
    }
    
            else if (input[i] == "t") {
              this.outputBa.push("5");
    }
    
            else if (input[i] == "z") {
              this.outputBa.push("6");
    }
    
            else if (input[i] == "u") {
              this.outputBa.push("7");
    }
    
            else if (input[i] == "i") {
              this.outputBa.push("8");
    }
    
            else if (input[i] == "o") {
              this.outputBa.push("9");
    }
    
            else if (input[i] == "p") {
              this.outputBa.push("0");
    }
    
                else if (input[i] == "a") {
                  this.outputBa.push("@");
    }
    
                else if (input[i] == "s") {
                  this.outputBa.push("#");
    }
    
                else if (input[i] == "d") {
                  this.outputBa.push("$");
    }
    
                else if (input[i] == "f") {
                  this.outputBa.push("_");
    }
    
                else if (input[i] == "g") {
                  this.outputBa.push("&");
    }
    
                else if (input[i] == "h") {
                  this.outputBa.push("-");
    }
    
                else if (input[i] == "j") {
                  this.outputBa.push("+");
    }
    
                else if (input[i] == "k") {
                  this.outputBa.push("(");
    }
    
                else if (input[i] == "l") {
                  this.outputBa.push(")");
    }
    
                    else if (input[i] == "y") {
                      this.outputBa.push("*");
    }
    
                    else if (input[i] == 'x') {
                      this.outputBa.push('"');
    }
    
                    else if (input[i] == "c") {
                      this.outputBa.push("'");
    }
    
                    else if (input[i] == "v") {
                      this.outputBa.push(":");
    }
    
                    else if (input[i] == "b") {
                      this.outputBa.push(";");
    }
    
                    else if (input[i] == "n") {
                      this.outputBa.push("!");
    }
    
                    else if (input[i] == "m") {
                      this.outputBa.push("?");
    }
    
                       else if (input[i] == " ") {
                        this.outputBa.push(" ");
    }
      }
      let outputJ = this.outputBa.join("");
  this.outputBa = outputJ
  console.log(outputJ);
  return outputJ;

    }
  }
}

</script>

<style scoped>

.eng {
  width: 50%;
  max-height: 1500px;
  padding-bottom: 5%;
  display: flex;
  flex-direction: column;
}

.ang {
  width: 50%;
  max-height: 1500px;
  padding-bottom: 5%;
  display: flex;
  flex-direction: column;
}
.btn {
  height: 120px;
}

input {
  font-size: 2em;
  width: 300px;
  height: 200px;
}



img {
  width: 20%;
}
</style>