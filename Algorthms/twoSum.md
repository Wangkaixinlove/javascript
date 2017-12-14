```js
/**
 * @param {number[]} nums
 * @param {number} target
 * @return {number[]}
 */

var twoSum = function(nums, target) {
    var arr=[];
    for(var i=0;i<nums.length;i++){
       for(var j=i;j<nums.length;j++){
           if(nums[i]+nums[j]==target && i!=j)
               {
               arr.push(i);
               arr.push(j);
               }
       }
    }
    return arr;
};
console.log(twoSum([2,3,4],6));
```