
1. Value vs. Reference Variable Assignment.  primitive type(number,string bool) vs object, function, Array
  let var1 = 'My string';
  let var2 = var1;
  var2 = 'My new string';
  
  let var1 = { name: 'Jim' }
  let var2 = var1;
  var2.name = 'John';
  
  
  
2.reduce 
  reduce((accumulator, currentValue, index, array) => { ... }, initialValue)



3.splice //remove or replace and/or add new item
  splice(start)
  splice(start, deleteCount)
  splice(start, deleteCount, item1)
  splice(start, deleteCount, item1, item2, itemN)
  
  
