# Write-a-Python-program-to-create-a-dictionary-from-two-lists-without-losing-duplicate-values

from collections import defaultdict
keys = ['Class-V', 'Class-VI', 'Class-VII', 'Class-VIII']
values = [1, 2, 2, 3]
my_dict = defaultdict(set)
for key, value in zip(keys, values):
 my_dict[key].add(value)
print(my_dict)
