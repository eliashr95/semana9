function incrementString(str) {
  let match = str.match(/\d+$/);
  if (!match) {
    return str + "1";
  }
  let num = match[0];
  let newNum = (parseInt(num) + 1).toString();
  while (newNum.length < num.length) {
    newNum = "0" + newNum;
  }
  return str.replace(/\d+$/, newNum);
}
