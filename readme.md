function pair(str) {
var array = str.split("");
  var results = [];
  
  array.reduce(function(acc, pre){
    if(pre === "A"){
      results.push(["A","T"]);
    } else if(pre === "T"){
      results.push(["T", "A"]);
    } else if(pre === "C"){
      results.push(["C","G"]);
    } else if (pre === "G"){
      results.push(["G","C"]);
    } 
  }, results);
  return results;
}

pair("GCG");
