fetch('https://nthieu2610.github.io/jsondemo/qlc4.json')
  .then(response => response.json())
  .then(data => {
    const jsonData = data;
    const inputElement = document.getElementById('ContentPlaceHolder1_hddListQuestion_ID_CAUHOI');
    const questionIdsString = inputElement.value;
    const questionIds = questionIdsString.split(',').filter(id => id !== '');

    const questionValues = {};
    questionIds.forEach((id, index) => {
      const value = jsonData[id];
      if (value) {
        questionValues[index + 1] = value;
      }
    });

    console.log(questionValues);
  })
  .catch(error => console.error('Error fetching JSON:', error));
