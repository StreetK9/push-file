
const { template } = require('@babel/core')

function minMedMax(n1, n2, n3) {
  let max
  let mid
  let min


//parameter max
  if (n1 > n2 && n1 > n3 ) {
   max = n1
  } else if (n2 > n3 && n2 > n1) {
  max = n2
  } else if(n3>n1 && n3>n2){
    max =n3
  }

//parameter อยู่ตรงกลาง
  if (n1 > n2 && n1 < n3 || n1>n3 && n1<n2) {
     mid = n1
  } else if (n2 > n3 && n2 < n1 || n2>n1 && n2<n3) {
    mid = n2
  }else if(n3>n1 && n3<n2 || n3>n2 && n3<n1){
    mid = n3

//ต้องซ้ำอยู่ตรงกลาง
  } else if (n1 == n2 && (n1||n2) < n3){  //(1,1,3)
    mid = n2
  }else if (n1 == n2 && (n1||n2) > n3){ //(3,1,1)
   mid = n2
  }else if (n2==n3 && (n2||n3) > n1){
    mid =n2
  }else if (n2==n3 && (n2||n3) < n1){
   mid =n2
}else if (n1==n3 && (n1||n3) > n2){
  mid = n1
}else if (n1==n3 && (n1||n3) < n2){
  mid = n1
}


  if (n1 < n2 && n1 < n3 ) {
    min = n1
  } else if (n2 < n1 && n2 < n3) {
    min = n2
  } else if (n3<n1){
    min = n3
  }

  let minMedMaxObj = { min: min, mid: mid, max: max }
  return minMedMaxObj
  
}
// console.log(minMedMax(85, 30, 1))
// console.log(minMedMax(10, 0, 20))
// console.log(minMedMax(-5, 0, 10))
// console.log(minMedMax( 5, 1, 1))
// console.log(minMedMax(-1, -8, 0))

module.exports = minMedMax
