# RotateArray-in-DSA-using-python
Rotating an array using python and java 
## 🔍 
This program rotates an array arr of size n to the left by `d` positions by shifting elements one-by-one and placing the first elements at the end.

## 💻 Code with Explanation and Dry Run

```python
def rotateArray(arr, d):
    n = len(arr)

    # ➤ Repeat rotation d times
    # Example: d = 3, n = 5

    # 1 2 3 4 5 = 4 5 1 2 3 
for i in range(d):

 # 1 2 3 4 5 = 4 5 1 2 3  


 # ➤ Left rotate by 1
        first = arr[0]  # Example: first = 1
        for j in range(n - 1):
            arr[j] = arr[j + 1]  # arr[0] = arr[1] → shift left
        arr[n - 1] = first  # Put first at end → arr[4] = 1


