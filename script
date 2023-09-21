var inputVal = document.getElementById("ContentPlaceHolder1_hddListQuestion_ID_CAUHOI").value;
var arr = inputVal.split(",");

fetch('https://nthieu2610.github.io/jsondemo/qa.json')
.then(response => response.json())
.then(data => {
    let results = [];
    for(let i = 0; i < 50; i++) {
        let currentVal = arr[i];
        let correspondingKey = data[currentVal];
        
        // Check if correspondingKey exists in the JSON data
        if(correspondingKey) {
            results.push((i+1) + correspondingKey);
        } else {
            results.push((i+1) + "-Unknown"); // If it doesn't exist, append 'unknown' 
        }
    }
    console.log(results);
});
