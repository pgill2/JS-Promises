# JS-Promises


# JS-Promises-Lab

<img src="https://i.imgur.com/PMyzlb1.png">

# JS Promises Lab

## Intro

You just learned about JavaScript Promises, both how to create them and how to consume promises returned by libraries such as Mongoose.

This lab will provide you with more practice using the promise syntax of Mongoose queries.

## Setup

Create a folder called `JS-Promises-Lab` inside your sandbox or the directory for your lab work, and create a file called **js-promises-lab.js** 

Alternatively, you can clone this repository and start working in the **js-promises-lab.js** file.


## Lab Requirements

1. Copy the following code & exercises into **js-promises-lab.js** (if you cloned this repo the file will already have it):

```js

let performers = [
  {name: 'Natalie Portman', born: '06-09-1981'},
  {name: 'Kevin Bacon', born: '07-08-1958'},
  {name: 'Tom Cruise', born: '07-03-1962'},
  {name: 'Brad Pitt', born: '12-18-1963'},
  {name: 'Emma Watson', born: '04-15-1990'},
  {name: 'Carrie Fisher', born: '10-21-1956'},
  {name: 'Mark Hamill', born: '09-25-1951'},
  {name: 'Harrison Ford', born: '07-13-1942'},
  {name: 'Jodie Foster', born: '11-19-1962'},
  {name: 'Matthew McConaughey', born: '11-04-1969'},
  {name: 'James Woods', born: '04-18-1947'},
  {name: 'Anne Hathaway', born: '11-12-1982'},
  {name: 'Bill Murray', born: '09-21-1950'},
  {name: 'Chevy Chase', born: '10-08-1943'},
  {name: 'Rami Malek', born: '05-12-1981'}
];

let movies = [
  {title: 'Contact', releaseYear: 1997, mpaaRating: 'PG', nowShowing: false},
  {title: 'Star Wars - A New Hope', releaseYear: 1977, mpaaRating: 'PG', nowShowing: false,
    reviews: [{content: 'The one that started it all!', rating: 5}]
  },
  {title: 'Interstellar', releaseYear: 2014, mpaaRating: 'PG-13', nowShowing: true,
    reviews: [{content: 'A fantastic sci-fi mind blower!', rating: 5}]
  },
  {title: 'Caddyshack', releaseYear: 1980, mpaaRating: 'R', nowShowing: false,
    reviews: [{content: 'Low-budget senseless comedy', rating: 4}, {content: 'Should not be the classic it is.', rating: 2}]
  },
  {title: 'Bohemian Rhapsody', releaseYear: 2018, mpaaRating: 'PG-13', nowShowing: true}
];



/*-- For each exercise below, write the code as described --*/

Promise.resolve().then(function() {

    console.log('HERE')
    // 1) Find all movie docs
    return movies  // remember to return the promise!
    
  }).then(function(result) {
    console.log('1): ', result)
    
    // 2) Find all performer docs
    
    return performers
  }).then(function(result) {
    console.log('2): ', result)
    
    // Follow the same .then structure used above from this point forward
    // Don't forget to console.log the exercise number also as shown above 
    // 3) Find all movies with an MPAA Rating of 'PG'
    
    PGMovies = movies.filter(movie => movie.mpaaRating === 'PG')
    return PGMovies
    // return movies.filter(movie => movie.mpaaRating === 'PG') ---> This is more concise
  
  }).then(function(result) {
      console.log('3): ', result)
  
    // 4) Find all movies that are still showing
    
    })


  // 5) Find all movies with an MPAA Rating of 'PG' or 'PG-13'


  // 6) Find the first movie found with a releaseYear of 2018


  // 7) Find all movies released after 1980
  

  // 8) Find all movies whose titles start with a 'C'
  

  // 9) Find the performer named 'Rami Malek'
  
  
  // 10) Find all performers born before 1980
  
  
  // 11) Find all performers whose name starts with a 'J'


.then(function() {
  process.exit();
});
```

2. Write the code for each exercise. Do not use a semicolon at the end of any `.then()`, otherwise the included `.then()` at the end of the code will not properly shut down the app.


## Hints

Use Filter and Find and other Array Iterator methods to complete the tasks

