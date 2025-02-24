+++
title = "Reproducible Research Experiments"
outputs = ["Reveal"]
+++

# Reproducible Research Experiments
## Martina Baiardi and Raphael Schwinger

---

# Table of Contents

1. Introduction to reproducible research meaning (**Martina**)
2. Reproducibility starts from development: build tools (gradle x JVM, Poetry x Python) and frameworks (hydra) (**Raphael**)
3. Basics of Containerization: Dockerfile and docker-compose (**Martina**)
4. Hands on a project: RL reproducible experiment setup using Poetry and Hydra (**Raphael**)
5. Cherry on the top: automation. GitHub, OSS proj, CI/CD pipelines, Github Actions, ... (**Martina**)


---

# Short guide to Markdown slides

---

# Headers

# H1
## H2
### H3
#### H4

---

# Text

normal text

`inline code`

*italic*

**bold**

**_emphasized_**

*__emphasized alternative__*

~~strikethrough~~

[link](http://www.google.com)

---

# Lists and enums

1. First ordered list item
1. Another item
    * Unordered sub-list.
    * with two items
        * another sublist
            1. With a sub-enum
            1. yay!
1. Actual numbers don't matter, just that it's a number
  1. Ordered sub-list
1. And another item.

---

# Inline images

![Alternative text](https://upload.wikimedia.org/wikipedia/commons/6/6c/Scavolino_innevata.jpg)

---

## Fallback to shortcodes for resizing

Autoresize specifying

* `max-w` (percent of parent element width) and/or `max-h` (percent of viewport height) as max sizes , and
* `width` and/or `height` as *exact* sizes (as percent of viewport size)

{{< figure src="https://upload.wikimedia.org/wikipedia/commons/6/6c/Scavolino_innevata.jpg" height="20">}}

---

## Multi-column slide

{{% multicol %}}{{% col %}}
Column 1
{{% /col %}}{{% col %}}
Column 2
{{% /col %}}{{% /multicol %}}

{{% multicol %}}
{{% col class="col-8" %}}
Larger columns using bootstrap
{{% /col %}}
{{% col %}}
[Link to bootstrap grid system](https://getbootstrap.com/docs/4.0/layout/grid/)
{{% /col %}}
{{% /multicol %}}

---

## Chart.js

{{< chart >}}
{
    type: 'bar',
    data: {
        labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
        datasets: [{
            label: 'Bar Chart',
            data: [12, 19, 18, 16, 13, 14],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
                'rgba(255, 206, 86, 0.2)',
                'rgba(75, 192, 192, 0.2)',
                'rgba(153, 102, 255, 0.2)',
                'rgba(255, 159, 64, 0.2)'
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)',
                'rgba(54, 162, 235, 1)',
                'rgba(255, 206, 86, 1)',
                'rgba(75, 192, 192, 1)',
                'rgba(153, 102, 255, 1)',
                'rgba(255, 159, 64, 1)'
            ],
            borderWidth: 1
        }]
    },
    options: {
        maintainAspectRatio: false,
        scales: {
            yAxes: [{
                ticks: {
                    beginAtZero: true
                }
            }]
        }
    }
}
{{< /chart >}}

---

## FontAwesome

<i class="fa-solid fa-mug-hot"></i>
<i class="fa-solid fa-lemon"></i>
<i class="fa-solid fa-flask"></i>
<i class="fa-solid fa-apple-whole"></i>
<i class="fa-solid fa-bacon"></i>
<i class="fa-solid fa-beer-mug-empty"></i>
<i class="fa-solid fa-pepper-hot"></i>

---

## Bootstrap 1

<div class="card w-100" >
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e9/View_of_Cesena_from_the_Abbey.jpg/1920px-View_of_Cesena_from_the_Abbey.jpg" class="card-img-top" alt="...">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

---

## Bootstrap 2

<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-secondary">Secondary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-warning">Warning</button>
<button type="button" class="btn btn-info">Info</button>
<button type="button" class="btn btn-light">Light</button>
<button type="button" class="btn btn-dark">Dark</button>

<button type="button" class="btn btn-link">Link</button>

---

## Low res, plain markdown

![](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6c/Scavolino_innevata.jpg/260px-Scavolino_innevata.jpg)

---

## Hi res, plain markdown

![](https://upload.wikimedia.org/wikipedia/commons/6/6c/Scavolino_innevata.jpg)

---

{{< slide background-image="https://upload.wikimedia.org/wikipedia/commons/6/6c/Scavolino_innevata.jpg" >}}

# Large images as background
## (May affect printing)

---


{{< slide background-video="https://github.com/DanySK/slides-2024-acsos-imageonomics/raw/master/content/nonnadir.mkv" background-video-loop="true" background-video-muted="true" background-opacity="0.95">}}

# Video background

---

# $$\LaTeX{}$$


Inline equations like $E=mc^2$

$$\frac{n!}{k!(n-k)!} = \binom{n}{k}$$

---

# Code snippets


```kotlin
val x = pippo
```

```go
package main

import "fmt"

func main() {
    fmt.Println("Hello world!")
}
```

---

# Tables

Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the
raw Markdown line up prettily. You can also use inline Markdown.

---

# Quotes

> Multiple
> lines
> of
> a
> single
> quote
> get
> joined

> Very long one liners of Markdown text automatically get broken into a multiline quotation, which is then rendered in the slides.

---

# Fragments

* {{< frag c="pluto" >}}
* {{< frag c="pluto" >}}
* {{< frag c="pluto" >}}

---

# Stacking images with Fragments
{{% multicol %}}
{{% col %}}
<p class="fragment" data-fragment-index="0">Pippo</p>
<p class="fragment" data-fragment-index="1">Pluto</p>
<p class="fragment" data-fragment-index="2">Paperino</p>
{{%/ col %}}

{{% col %}}
<div class="r-stack">
  <img
    class="fragment current-visible"
    data-fragment-index="0"
    src="https://www.topolino.it/wp-content/uploads/2019/12/pippointera.png"
    width="450"
    height="300"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="1"
    src="https://www.topolino.it/wp-content/uploads/2019/12/plutointera.png"
    width="300"
    height="450"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="2"
    src="https://it.wikifur.com/w/images/thumb/6/6f/Donald_Duck.png/362px-Donald_Duck.png"
    width="400"
    height="400"
  />
</div>
{{%/ col %}}

{{%/ multicol %}}


---

# Keystrokes

<kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>Del</kbd>