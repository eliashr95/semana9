function validParentheses(str) {
  return (
    str.split("").reduce((acc, val) => {
      if (val === "(") {
        acc++;
      } else if (val === ")") {
        acc--;
        if (acc < 0) {
          acc = NaN;
        }
      }
      return acc;
    }, 0) === 0
  );
}
