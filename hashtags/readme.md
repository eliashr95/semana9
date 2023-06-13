function generateHashtag(str) {
  if (str.length === 0) return false;
  let hashtag = str
    .split(" ")
    .reduce(
      (acc, val) => (acc += val.charAt(0).toUpperCase() + val.slice(1)),
      "#"
    );
  if (hashtag.length > 140) return false;
  return hashtag;
}
