### FancySlider-DebuggingTask

#### Error-01: Search Field
const getImages = (query) => {
  fetch(`https://pixabay.com/api/?key=${KEY}=${query}&image_type=photo&pretty=true`)
    .then(response => response.json())
    .then(data => showImages(data.hits)) //Solved this line
    .catch(err => console.log(err))
}

#### Error-02: Slider Creation
 <input class="form-control" id="duration" placeholder="slider change duration"> <!--Solved here the id doration to duration>

 #### Error-03: Duration Time Must Not Be Negative
 const positiveDuration = Math.abs(duration); // Convert a negative value into a positive value;