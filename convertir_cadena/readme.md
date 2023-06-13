function toCamelCase(str) {
  if (str === "") return "";
  let words = str.split("");
  return words.reduce((acc, val, i) => {
    if (val === "-" || val === "_") {
      return acc + words[i + 1].toUpperCase();
    } else {
      return acc + val;
    }
  }, words[0]);
}
