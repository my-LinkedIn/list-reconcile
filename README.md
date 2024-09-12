# list-reconcile
List reconciliation script using Python

## Source code

```python
def find_unique_elements(list1, list2):
    """
    Find the elements that are not shared between two lists.

    Args:
        list1 (list): The first list.
        list2 (list): The second list.

    Returns:
        tuple: A tuple containing two lists. The first list contains elements unique to list1,
            and the second list contains elements unique to list2.
    """
    # Convert the lists to sets for efficient lookups
    set1 = set(list1)
    set2 = set(list2)

    # Find the elements that are not shared between the two lists
    unique_to_list1 = [element for element in list1 if element not in set2]
    unique_to_list2 = [element for element in list2 if element not in set1]

    return unique_to_list1, unique_to_list2

def main():
    # Define two random lists for illustration
    list1 = [105, 111, 117, 123, 129, 135, 141, 147, 153, 159, 165, 171, 177, 183, 189, 195, 201, 207, 219, 225, 249, 255, 261, 267, 279, 285, 291, 297, 405, 411, 417, 429, 441, 447, 459, 465, 471, 477, 489, 495, 501, 507, 519, 525, 549, 555, 561, 567, 579, 585, 591, 597, 609, 615, 621, 627, 645, 651, 657, 669, 675, 681, 687, 699, 705, 711, 717, 729, 741, 747, 759, 765, 771, 777, 789, 795, 801, 807, 819, 825, 849, 855, 861, 867, 879, 885, 891, 897, 909, 915, 921, 927, 945, 951, 957, 969, 975, 981, 987, 999]
    list2 = [105, 111, 117, 129, 141, 147, 159, 165, 171, 177, 189, 195, 201, 207, 219, 225, 249, 255, 261, 267, 279, 285, 291, 297, 405, 411, 417, 429, 441, 447, 459, 465, 471, 477, 489, 495, 501, 507, 519, 525, 549, 555, 561, 567, 579, 585, 591, 597, 609, 615, 621, 627, 645, 651, 657, 669, 675, 681, 687, 699, 705, 711, 717, 729, 741, 747, 759, 765, 771, 777, 789, 795, 801, 807, 819, 825, 849, 855, 861, 867, 879, 885, 891, 897, 909, 915, 921, 927, 945, 951, 957, 969, 975, 981, 987, 999]

    # Find the elements that are not shared between the two lists
    unique_to_list1, unique_to_list2 = find_unique_elements(list1, list2)

    # Print the results
    print("Elements unique to the first list:")
    for element in unique_to_list1:
        print(element)

    print("Elements unique to the second list:")
    for element in unique_to_list2:
        print(element)

if __name__ == "__main__":
    main()
```

## Output

```text
```
