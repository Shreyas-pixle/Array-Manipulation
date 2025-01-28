def perform_operations_and_find_max(arr, operations):
    for i in range(len(arr)):
        arr[i] += operations[i]
    
    max_value = max(arr)
    return max_value

n = int(input("Enter the number of elements in the array: "))
arr = []
print("Enter the elements of the array:")
for i in range(n):
    arr.append(int(input(f"Element {i + 1}: ")))
operations = []
print("Enter the operations (values to add to each element):")
for i in range(n):
    operations.append(int(input(f"Operation {i + 1}: ")))

max_value = perform_operations_and_find_max(arr, operations)
print("The maximum value after all operations is:", max_value)
