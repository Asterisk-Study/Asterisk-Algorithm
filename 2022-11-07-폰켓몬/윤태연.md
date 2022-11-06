function solution(nums) {
  // 1. 종류 최대 nums가지면 nums/2 정도가 최댓값
  // 2. 중복값 있다면 없애고(set) 길이 구하기(size)
  // 3. 최댓값이랑 set 비교해서 set.size가 크다면 무얼 조합해도 최댓값을 넘지 않기에 최댓값 반환, 중복이 많아 set.size가 작다면 size반환

  // 1
  const numsMax = nums.length / 2;
  // 2
  const pokemonSet = new Set(nums);
  // 3
  return pokemonSet.size > numsMax ? numsMax : pokemonSet.size;
}
