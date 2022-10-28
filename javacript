function tytul() {
    var pytanie = "Jaki geld dajesz na paliwo?";
    document.getElementById("nazwa").innerHTML = pytanie;
  }
  window.onload = tytul;



  function sprowdzej()
  {
    
    var x = document.forms["myForm"]["km"].value;
    if (isNaN(x)) {
      document.getElementById("nazwa").innerHTML = `<font color="red">Chyba Ktoś sie ciulnoł</font>`;
      return false;
      
    }

    if (x == null || x == "") {
      document.getElementById("nazwa").innerHTML = `<font color="red">A podosz te kilosy?</font>`;
      return false;
      
    }
    
    var y = document.forms["myForm"]["cena"].value;
    if (isNaN(y)) {
      document.getElementById("nazwa").innerHTML = `<font color="red">Nie bulisz w złotkach?</font>`;
      return false;
      if (y= Number){
        document.getElementById("nazwa").innerHTML = `<font color="green">dane</font>`;
      }
    }
    if (y == null || y == "") {
      document.getElementById("nazwa").innerHTML = `<font color="red">Leją Ci za friko</font>`;
      return false;
    }
    
    var z = document.forms["myForm"]["spalanie"].value;
    if (isNaN(z)) {
      document.getElementById("nazwa").innerHTML = `<font color="red">Weź nie rób mnie za bozna!</font>`;
      return false;
    }
    if (z == null || z == "") {
      document.getElementById("nazwa").innerHTML = `<font color="red">Ino nie godej że jeżdzisz na luft!</font>`;
      return false;
    }
    else{
      document.getElementById("nazwa").innerHTML = `<font color="green">DANE POPRAWNE/font>`;
    }
  
  return true;
}





function koszt() {

var km = document.getElementById("km").value;
var rounded = Math.round(km * 10) / 10;

var cena = document.getElementById("cena").value;
var rounded = Math.round(cena * 10) / 10

var spalanie = document.getElementById("spalanie").value;
var rounded = Math.round(spalanie * 10) / 10

if (km * spalanie / 100 * cena <=10) {
      document.getElementById("nazwa").innerHTML = `<font color="red">Ciulosz czy mało jeździsz?</font>`;
      return false;     
    }
    if (km * spalanie / 100 * cena >=10000) {
      document.getElementById("nazwa").innerHTML = `<font color="red">Kto bagatemu zabroni ?</font>`;
      return false;     
    }

document.getElementById("nazwa").innerHTML = (`<font color="green">Pieronie ... ze </font>`+ km * spalanie / 100 * cena + `<font color="green"> zlotków!</font>`);
document.getElementById("reset").style.display = "block";

}

function validowanie1() {
if (sprowdzej()) {
  document.getElementById("nazwa").innerHTML = `<font color="green">Ja, tera je dobrze</font>`;  }
return false;
}


function validowanie2() {
if (sprowdzej()) {
  koszt();  
} else {
  document.getElementById("nazwa").innerHTML = `<font color="red">Poprow bo nie idzie</font>`;  
}

}