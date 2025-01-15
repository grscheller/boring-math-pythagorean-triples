# Daddy's boring math library - Pythagorean triple module

Module to generate and explore Pythagorean triples.

Part of the "Boring Math" PyPI **bm** namespace for mathematical hobby
projects.

* [bm.pythagorean-triples](#pythagorean-triples)

* **Repositories**
  * [bm.pythagorean-triples][1] project on *PyPI*
  * [Source code][2] on *GitHub*
* **Detailed documentation**
  * [Detailed API documentation][3] on *GH-Pages*

## Library Modules

### Pythagorean Triples Module

* Pythagorean Triple Class
  * Method **Pythag3.triples**(a_start: int, a_max: int, max: Optional[int]) -> Iterator[int]
    * Returns an iterator of tuples of primitive *Pythagorean* triples
  * A Pythagorean triple is a tuple in positive integers (a, b, c)
    * such that `a² + b² = c²`
    * `a, b, c` represent integer sides of a right triangle
    * a *Pythagorean* triple is primitive if gcd of `a, b, c` is `1`
  * Iterator finds all primitive Pythagorean Triples
    * where `0 < a_start <= a < b < c <= max` where `a <= a_max`
    * if `max = 0` find all theoretically possible triples with `a <= a_max`

---

## CLI Applications

### Pythagorean triple CLI script

Geometrically, a *Pythagorean* triangle is a right triangle with
positive integer sides.

#### CLI program **pythag3**

* Generates primitive Pythagorean triples
  * A primitive Pythagorean triple is a 3-tuple of integers `(a, b, c)` such that
    * `a³ + b³ = c³` where `a,b,c > 0` and `gcd(a,b,c) = 1`
  * The integers `a, b, c` represent the sides of a right triangle
* **Usage:** `pythag3 [m [n [max]]`
  * 3 args print all triples with `m <= a <= n` and `a < b < c <= max`
  * 2 args print all triples with `m <= a <= n`
  * 1 arg prints all triples with `a <= m`
  * 0 args print all triples with `3 <= a <= 100`

---

[1]: https://pypi.org/project/bm.pythagorean-triples/
[2]: https://github.com/grscheller/bm-pythagorean-triples/
[3]: https://grscheller.github.io/boring-math-docs/pythagorean-triples
