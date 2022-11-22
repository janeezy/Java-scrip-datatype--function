# Java-scrip-datatype--function
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>profile page</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section class="gridcontainer">
      <button id="button_A">Press me</button>
      <h3 id="heading_A">follow the instructions</h3>
    </section>

    <script src="app.js"></script>
  </body>
</html>

* {
  background-color: rgb(31, 42, 38);
}

.gridcontainer {
  align-items: center;
  display: flex;
  flex-grow: inherit;
  flex-direction: column;
  font-weight: 500;
  margin: 40px;
  padding: 10px;
}

#button_A {
  color: azure;
  background: darkgoldenrod;
  padding: 30px;
  margin: 80px;
  display: grid;
  flex-direction: column-reverse;
  border: 10px;
}

#heading_A {
  color: white;
  font-size: x-large;
  font-family: monospace;
}
const buttonA = document.querySelector('#button_A');
const headingA = document.querySelector('#heading_A');

buttonA.onclick = () => {
  const name = prompt('What is your name?');
  alert(`Hello ${name}, nice to see you!`);
  headingA.textContent = `Welcome ${name}`;
};
