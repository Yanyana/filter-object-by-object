# filterObjectByObject
var x = [
 {"val": 1, "text": "a"},
 {"val": 2, "text": "b"},
 {"val": 3, "text": "c"},
 {"val": 4, "text": "d"},
 {"val": 5, "text": "e"}
],
 y = [
  {"val": 1, "text": "a"},
  {"val": 4, "text": "d"}
];

var yFilter = y.map(itemY => { return itemY.val; });
var filteredX = x.filter(itemX => !yFilter.includes(itemX.val));

console.log(JSON.stringify(filteredX));