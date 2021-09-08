# assignment2-pandiri
# Pandiri Govinda Reddy
## GOA

GOA is the **best place** to enjoy as it is the only **place** where it contains most number of **beaches**.

***

# Navigation From Maryville To Fairborn

1. First we have to reach Kansas airport. 
2. Kansas to Indianapolis which is the first stop point. 
3. Have to wait for 2 hours, then take second flight from Indianapolis to Dayton.
    1. Dayton is located in Ohio state. 
4. Atlast have to take road journey from Dayton to Fairborn about 25 minutes of travel. 

# Favourite Things To Carry While Travelling To Favourite Place 

* Camera
* clothes
* sunglasses
* Tabs

---

**[About Me](AboutMe.md)**

---

# My Favourite Food Items

These are the best food items that you can find here in USA

| Item  | Location  | Cost  |   
|---|---|---|
| Biryani  |  Bawarchi |  $12.99 |   
|  Ice cream | Arun  |  $2.55 |   
| Tacos  |Tacobell   |$4.99   |
|   Burger| Burger king  |  $2.99 |

***

# Pithy Quotes

>Beauty in things exists in the mind which contemplates them. - *David Hume*

>There is no excellent beauty that hath not some strangeness in the proportion. - *Francis Bacon*

---

# Catalan Numbers Algorithm

In combinatorial mathematics, the Catalan numbers form a sequence of natural numbers that occur in various counting problems, often involving recursively defined objects. They are named after the Belgian mathematician Eugène Charles Catalan (1814–1894).The first Catalan numbers for n = 0, 1, 2, 3, ... are
1, 1, 2, 5, 14, 42, 132, 429, 1430, 4862, 16796, 58786, ...

Link: <https://en.wikipedia.org/wiki/Catalan_number>

```
const int MOD = ....
const int MAX = ....
int catalan[MAX];
void init() {
    catalan[0] = catalan[1] = 1;
    for (int i=2; i<=n; i++) {
        catalan[i] = 0;
        for (int j=0; j < i; j++) {
            catalan[i] += (catalan[j] * catalan[i-j-1]) % MOD;
            if (catalan[i] >= MOD) {
                catalan[i] -= MOD;
            }
        }
    }
}
```

Link: <https://cp-algorithms.com/combinatorics/catalan-numbers.html>