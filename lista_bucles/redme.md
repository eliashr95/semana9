function processData(data) {
  let product = 1;

  for (let i = 0; i < data.length; i++) {
    let result = data[i][0] - data[i][1];

    product *= result;
  }
  return product;
}
