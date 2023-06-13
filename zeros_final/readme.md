function moveZeros(nums) {
  let nonZero = nums.filter((val) => val !== 0);
  let zeros = nums.filter((val) => val === 0);
  return nonZero.concat(zeros);
}
