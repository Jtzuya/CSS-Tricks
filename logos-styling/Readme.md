###### Inconsistent sized logos... fixed!

**Before:**
<img src="https://github.com/Jtzuya/https://github.com/Jtzuya/css-styling-tricks/logos-styling/master/assets/before.png" width="250" height="auto"/>

<sup>As you can see from the above image. Some images doesn't have same background/height</sup>

```css
 /* giving all them the same length with the combination of width + aspect ration (bread and butter)*/
.photos img {
    width: 15%;
    aspect-ratio: 3/2;

    /* object fit contain to fix the image(s) that are stretched */
    object-fit: contain;

    /* lastly, to remove the white background... By using mix blend mode of color burn that do the magic */
    mix-blend-mode: color-burn;
}
```

**After:**
<img src="https://github.com/Jtzuya/https://github.com/Jtzuya/css-styling-tricks/logos-styling/master/assets/after.png" width="250" height="auto"/>

<sub>Use these combinations of css properties on your next project!</sub>

<sup>Credits to: [@Wesbos](https://www.youtube.com/@WesBos) and check out his youtube channel</sup>


### Uncommon CSS Properties crossbrowser support
[Aspect Ratio](https://caniuse.com/?search=mix-blend-mode)
[Mix Blend Mode](https://caniuse.com/?search=aspect-ratio)
[Object Fit](https://caniuse.com/?search=object-fit)