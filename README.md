### FancySlider-DebuggingTask

#### Error-01: Search Field
const getImages = (query) => {
  fetch(`https://pixabay.com/api/?key=${KEY}=${query}&image_type=photo&pretty=true`)<br>
    .then(response => response.json())<br>
    .then(data => showImages(data.hits)) //Solved this line <br>
    .catch(err => console.log(err))
}

#### Error-02: Slider Creation
 - In index.html file fixing the id 'doration' to 'duration' <br>

 #### Error-03: Duration Time Must Not Be Negative
 const positiveDuration = Math.abs(duration); // Convert a negative value into a positive value;<br>

#### Feature-01: Enter KeyPress Worked
- Using 'keypress() and click()' method.

#### Live-Demo: https://muhammed-nayeem.github.io/FancySlider-DebuggingTask/index.html