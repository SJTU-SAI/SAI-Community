# Introduction to Programming

Hello world, it is C++!

``` py title="bubble_sort.py"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
    # (1)
    # You can add annotations here!
```

<!-- 
``` yaml
theme:
  features:
    - content.code.annotate # (1)
``` -->

1.  😊 I'm a code annotation! I can contain `code`, __formatted
    text__, images, ... basically anything that can be written in Markdown.


The `#!python range()` function is used to generate a sequence of numbers.