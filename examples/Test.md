---
marp: true
theme: haskell
class: 
  - invert
header: 'test header'
footer: 'test footer'
math: mathjax

style: |
  .columns {
    display: grid;
    gap: 1rem;
  }

  .columns-2 {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }
---
<!-- _class: invert lead-invert-->
# Intro slide
made by test

---
# Content
- Text
  - Single coloumn and dual
- Code
- Image
  - Single
- Image and text
- Background

---
# Text single coloumn
Here are some text in a single coloumn
Next line

---
# Text multiple coloumn
<div class="columns columns-2">
<div>

## Column 1
Some text

</div>
<div>

## Column 2
Some more text

</div>
</div>

---
# Code
```rust
#[derive(Debug)]
pub enum State {
    Start,
    Transient,
    Closed,
}

impl From<&'a str> for State {
    fn from(s: &'a str) -> Self {
        match s {
            "start" => State::Start,
            "closed" => State::Closed,
            _ => unreachable!(),
        }
    }
}}
```

---
# Single image
![width:8in](wide.bmp)

---
# Image and text
![bg right height:5in](narrow2.bmp)

---
<!-- _color: black-->
# Background
![bg contain blur](wide.bmp)