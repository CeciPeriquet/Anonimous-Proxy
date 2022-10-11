# FINAL EVALUATION

The first module of Adalab Web Development Bootcamp it´s ending and this is the final exam we have to pass.

## Statement

We had to create a **responsive website** (with different zeplin desings for _mobile, tablet and desktop version_) and had to include the following:

- Sass
- Both Flexbox and CSS Grid
- Mediaqueries
- Transitions (an animation would be a BONUS)

## Technology

First thing to do was cloning the repository and add the template from **ADALAB STARTER KIT**, and then `npm install` to create _node_modules_ folder and start working with _node.js_ and _gulp_.

From now on we're going to use this template, so we won´t use Live Server but `npm start` to check changes on our browser (and use our beloved **DevTools**).

## A Bit of Story and Code

Before jumping over my keyboard to write code, I used _excalidraw.com_ to try to figure out the HTML structure of the website, as our teachers do. (As you can see I considered the hero image as a part of the header, but I guess in this case there's no right or wrong, it's just a point of view).

I created the whole HTML structure in `index.html` but then used partials for the different layouts of the site `<header> <main> and <footer>` basically, as afterwards I'd do with SASS styles.

First thing I set in `.scss` document was the variables, int this case I only used variables for the colors that the zeplin design gave us (althought I could have also used variables for the fonts).

As with the html layout, in this project I'm working with SCSS partials that, as you probably know (sorry, I'm a newby, first README.MD ever) have to be imported to the `main.scss` with the following commands:

````
@import 'core/variables';
@import 'core/reset';
@import 'layout/header';
@import 'layout/section1';
@import 'layout/section2';
@import 'layout/footer';```
````

As for the `_reset.scss` I didn't use a reset sheet (as I did in other school projects) felt just happy with:

```
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  list-style: none;
  text-decoration: none;
}
```

As we have to work with SASS, I've been using `nesting` (and at some point a bit of `BEM` when giving _classnames_) including `mediaqueries`:

```
 <section class="main__section1">
    <small class="main__section1-small">Insomnia tips</small>
    <h2 class="main__section1-title">Looking through a window</h2>
    <p class="main__section1-text">
      Donec accumsan, nulla ut volutpat porttitor, quam odio tempus felis, at luctus ex diam nec lectus. Vivamus semper sodales rutrum.
    </p>
    <a href="#" class="main__section1-link">Go</a>
  </section>
```

```
.main__section1 {

    @media all and (min-width: 768px) {

    }
    @media all and (min-width: 1200px) {

    }

    &-small {

        @media all and (min-width: 1200px) {

        }
    }

    &-title {

        @media all and (min-width: 768px) {

        }
        @media all and (min-width: 1200px) {

        }
    }

    &-text {

        @media all and (min-width: 768px) {

        }

    }
}
```

I kind of like them and hate them at the same time, it might be easier at some point but not with so less time to switch your brain from reglular CSS to SASS (_ahhh, bootcamps..._). I would have loved to add `mixins` but hadn't enought time.

I have to say that I love Flex, and I'm still understanding Grid, so, for now I'm **#teamFlex**

I really wanted to animate some stuff (as I used to be a tv worker, _video is my passion_) but I didn't have time enough to do a _super amazing awesome one_ (mainly because I learned abput the last day, trying to get everything done) so I made a simple one just to try it and start learning about it. I also used some regular transitions for other buttons.

## The Result

You can take a look of how it ended up in Github Pages: http://beta.adalab.es/modulo-1-evaluacion-final-CeciPeriquet/

Btw, don't look to much to my code, **it hasn't been aprooved yet...** (_oh, Hi Teacher!_)

## And, please, don´t forget:

```
npm run docs
git add -A
git commit -m ""
git push
*/ GO HAVE A BEER, YOU DESERVE IT /*
```
