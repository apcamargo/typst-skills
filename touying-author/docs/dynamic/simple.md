---
sidebar_position: 1
---

# Simple Animations

Touying provides two markers for simple animation effects: `#pause` and `#meanwhile`.

## pause

The purpose of `#pause` is straightforward – it separates the subsequent content into the next subslide. You can use multiple `#pause` to create multiple subslides. Here's a simple example:

```typst
#slide[
  First #pause Second

  #pause

  Third
]
```

![image](https://github.com/touying-typ/touying/assets/34951714/a3bed1d3-e660-456d-8a54-a914436f43bf)

This example will create three subslides, gradually revealing the content.

As you can see, `#pause` can be used inline or on a separate line.

## meanwhile

In some cases, you may need to display additional content simultaneously with `#pause`. In such cases, you can use `#meanwhile`.

```typst
#slide[
  First
  
  #pause
  
  Second

  #meanwhile

  Third

  #pause

  Fourth
]
```

![image](https://github.com/touying-typ/touying/assets/34951714/24ca19a3-b27c-4d31-ab75-09c37911e6ac)

This example will create only two subslides, with "First" and "Third" displayed simultaneously, and "Second" and "Fourth" displayed simultaneously.