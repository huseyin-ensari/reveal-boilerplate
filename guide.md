### Secret Notes

```html
<section>
  <h2>Some Slide</h2>

  <aside class="notes">
    Shhh, these are your private notes 📝
  </aside>
</section>
```

Add notes. And press `s` to open the notes window.

----

### Animation

```html
<section>
  <section data-auto-animate>
    <h1>Implicit</h1>
  </section>
  <section data-auto-animate>
    <h1>Implicit</h1>
    <h1>Animation</h1>
  </section>
</section>
```

#### Code 

```html
<section data-auto-animate>
  <pre data-id="code-animation"><code data-trim data-line-numbers>
    let planets = [
      { name: 'mars', diameter: 6779 },
    ]
  </code></pre>
</section>
<section data-auto-animate>
  <pre data-id="code-animation"><code data-trim data-line-numbers>
    let planets = [
      { name: 'mars', diameter: 6779 },
      { name: 'earth', diameter: 12742 },
      { name: 'jupiter', diameter: 139820 }
    ]
  </code></pre>
</section>
<section data-auto-animate>
  <pre data-id="code-animation"><code data-trim data-line-numbers>
    let circumferenceReducer = ( c, planet ) => {
      return c + planet.diameter * Math.PI;
    }

    let planets = [
      { name: 'mars', diameter: 6779 },
      { name: 'earth', diameter: 12742 },
      { name: 'jupiter', diameter: 139820 }
    ]

    let c = planets.reduce( circumferenceReducer, 0 )
  </code></pre>
</section>
```

#### Elements Matched

```html
<section data-auto-animate>
  <div data-id="box" style="height: 50px; background: salmon;"></div>
</section>
<section data-auto-animate>
  <div data-id="box" style="height: 200px; background: blue;"></div>
</section>
```

----

### Transition

```html
<section data-transition="slide">
    and on …
</section>
```

`none`, `fade`, `slide`, `convex`, `concave`, `zoom`

-----


### Code

```html
<pre><code data-line-numbers data-ln-start-from="7">
    var a = 10;
</code></pre>
```

- `data-line-numbers="3,8-10"`
- `ddata-line-numbers="3-5|8-10|13-15"`
- `data-line-numbers` | `data-ln-start-from="7"`

---- 

### Background

`data-background-color="#ff5d37"`

` data-background="image.png" data-background-repeat="repeat" data-background-size="100px"`

----

### Layout

```html
<h2 class="r-fit-text">FIT TEXT</h2>
<h2 class="r-fit-text">CAN BE USED FOR MULTIPLE HEADLINES</h2>
```

- `<h2 class="r-fit-text">BIG</h2>`
- `<img class="r-stretch" src="/images/slides-symbol-512x512.png">`

----

### Media

```html
<section>
  <img data-src="image.png">
  <iframe data-src="https://hakim.se"></iframe>
  <video>
    <source data-src="video.webm" type="video/webm" />
    <source data-src="video.mp4" type="video/mp4" />
  </video>
</section>
```