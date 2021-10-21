function partition(arr, lb, ub){
  
  pivot = arr[lb];
  start = lb;
  end = ub;
  
  while(start<end){
    
    while(arr[start]<=pivot && start<end){
      start++;
    }
    
    while(arr[end]>pivot){
      end--;
    }
    
    
    if(start<end){
      temp = arr[start];
      arr[start] = arr[end];
      arr[end] = temp;
    }
  }
  
  temp = arr[lb];
  arr[lb] = arr[end];
  arr[end] = temp;
  
  return end;
  
}

function quickSort(arr, start, end){
  
  if(start<end){
    pivotIndex = partition(arr, start, end);
    quickSort(arr, start, pivotIndex-1);
    quickSort(arr, pivotIndex+1, end);
  }
  
}

arr = [1000,54,36,12,78,99,21,12]

quickSort(arr, 0, arr.length-1);

console.log(arr);

