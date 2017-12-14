给定一个整数数组，返回两个数字的索引，使它们加起来成为一个特定的目标。  

您可能会认为每个输入都只有一个解决方案，而且您可能不会使用相同的元素两次。  

例：  
给定nums = [2,7,11,15]，目标= 9，  

由于nums [ 0 ] + nums [ 1 ] = 2 + 7 = 9，  
返回[ 0，1 ]。  
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
