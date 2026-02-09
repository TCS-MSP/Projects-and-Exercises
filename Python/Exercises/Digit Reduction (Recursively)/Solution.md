```python
# Returns the highest value in the fully reduced list
def main(insert_list):
  fully_reduced = insert_list;
  while(find_max(fully_reduced) >= 10):
    fully_reduced = helper_function(fully_reduced);
  return find_max(fully_reduced)

# Reduces the list
def helper_function(insert_list):
  copy = insert_list;
  final = []
  for item in copy:
    curr_val = item;
    deduced = 0;
    while(curr_val > 0):
      additive = curr_val % 10
      deduced += additive;
      curr_val -= additive;
      curr_val /= 10;
    final.append(deduced);
  return final

# Finds max value in a list
def find_max(insert_list):
  answer = -1000;
  for item in insert_list:
    if item > answer:
      answer = item;
  return answer

ex1 = [12345, 6789, 10111213]
ex1 = []
print(main(ex1))
```
