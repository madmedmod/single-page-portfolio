<template>
  <div>
    <head>
      <meta charset="utf-8" />
      <meta http-equiv="X-UA-Compatible" content="IE=edge" />
      <title>Survey Form - 2nd FCC RWD Project</title>
      <meta name="viewport" content="width=device-width, initial-scale=1" />
      <link rel="stylesheet" type="text/css" media="screen" href="main.css" />
      <script src="main.js"></script>
    </head>
    <body>
      <div id="header">
        <h1 id="title">Survey Form</h1>
      </div>

      <div id="form-outer">
        <p id="description">This is a survey form</p>
        <form id="survey-form">
          <div class="rowTab">
            <div class="labelTab">
              <label id="name-label" for="name">Name:</label>
            </div>
            <div class="inputTab">
              <input
                id="name"
                class="input-field"
                type="text"
                required
                placeholder="You name here"
              />
            </div>
          </div>

          <div class="rowTab">
            <div class="labelTab">
              <label id="email-label" for="email">Email:</label>
            </div>
            <div class="inputTab">
              <input
                id="email"
                class="input-field"
                type="email"
                required
                placeholder="You email here"
              />
            </div>
          </div>

          <div class="rowTab">
            <div class="labelTab">
              <label id="number-label" for="number">Age:</label>
            </div>
            <div class="inputTab">
              <input
                id="number"
                class="input-field"
                type="number"
                min="1"
                max="150"
                placeholder="How old are you?"
              />
            </div>
          </div>

          <div class="rowTab">
            <div class="labelTab">
              <label id="">A role you're so passionate about:</label>
            </div>
            <div class="inputTab">
              <select id="dropdown" name="selection" class="dropdown">
                <option disabled value>Choose one</option>
                <option value="front-end">Front-End Developer</option>
                <option value="back-end">Back-End Developer</option>
                <option value="full-stack">Full-Stack Developer</option>
                <option value="mobile">Mobile Developer</option>
                <option value="desktop">Software Engineer</option>
                <option value="other">Other than these</option>
                <option value="all">I love them all</option>
              </select>
            </div>
          </div>

          <div class="rowTab">
            <div class="labelTab">
              <label id="" for="progLang"
                >Programming Language you love :</label
              >
            </div>
            <div class="inputTab">
              <ul style="list-style: none;">
                <li class="checkbox">
                  <label
                    ><input
                      name="checkbox-buttons"
                      value="1"
                      type="checkbox"
                      class="codingLove"
                    />Ruby</label
                  >
                </li>
                <li class="checkbox">
                  <label
                    ><input
                      name="checkbox-buttons"
                      value="2"
                      type="checkbox"
                      class="codingLove"
                    />R</label
                  >
                </li>
                <li class="checkbox">
                  <label
                    ><input
                      name="checkbox-buttons"
                      value="3"
                      type="checkbox"
                      class="codingLove"
                    />Phyton</label
                  >
                </li>
                <li class="checkbox">
                  <label
                    ><input
                      name="checkbox-buttons"
                      value="4"
                      type="checkbox"
                      class="codingLove"
                    />Javascript</label
                  >
                </li>
                <li class="checkbox">
                  <label
                    ><input
                      name="checkbox-buttons"
                      value="5"
                      type="checkbox"
                      class="codingLove"
                    />Java</label
                  >
                </li>
                <li class="checkbox">
                  <label
                    ><input
                      name="checkbox-buttons"
                      value="6"
                      type="checkbox"
                      class="codingLove"
                    />Kotlin</label
                  >
                </li>
                <li class="checkbox">
                  <label
                    ><input
                      name="checkbox-buttons"
                      value="7"
                      type="checkbox"
                      class="codingLove"
                    />PHP</label
                  >
                </li>
                <li class="checkbox">
                  <label
                    ><input
                      name="checkbox-buttons"
                      value="8"
                      type="checkbox"
                      class="codingLove"
                    />React-native</label
                  >
                </li>
                <li class="checkbox">
                  <label
                    ><input
                      name="checkbox-buttons"
                      value="9"
                      type="checkbox"
                      class="codingLove"
                    />C++</label
                  >
                </li>
                <li class="checkbox">
                  <label
                    ><input
                      name="checkbox-buttons"
                      value="10"
                      type="checkbox"
                      class="codingLove"
                    />Perl</label
                  >
                </li>
                <li class="checkbox">
                  <label
                    ><input
                      name="checkbox-buttons"
                      value="11"
                      type="checkbox"
                      class="codingLove"
                    />Swift</label
                  >
                </li>
                <li class="checkbox">
                  <label
                    ><input
                      name="checkbox-buttons"
                      value="12"
                      type="checkbox"
                      class="codingLove"
                    />Objective-C</label
                  >
                </li>
                <li class="checkbox">
                  <label
                    ><input
                      name="checkbox-buttons"
                      value="13"
                      type="checkbox"
                      class="codingLove"
                    />Erlang</label
                  >
                </li>
                <li class="checkbox">
                  <label
                    ><input
                      name="checkbox-buttons"
                      value="14"
                      type="checkbox"
                      class="codingLove"
                    />Others that not listed</label
                  >
                </li>
              </ul>
            </div>
          </div>

          <div class="rowTab">
            <div class="labelTab">
              <label id="" for="codingLove"
                >How much do you like to code?</label
              >
            </div>
            <div class="inputTab">
              <ul style="list-style: none;">
                <li class="radio">
                  <label
                    ><input
                      name="radio-buttons"
                      value="1"
                      type="radio"
                      class="codingLove"
                    />Deeply in love</label
                  >
                </li>
                <li class="radio">
                  <label
                    ><input
                      name="radio-buttons"
                      value="2"
                      type="radio"
                      class="codingLove"
                    />Just so-so</label
                  >
                </li>
                <li class="radio">
                  <label
                    ><input
                      name="radio-buttons"
                      value="3"
                      type="radio"
                      class="codingLove"
                    />Nah...</label
                  >
                </li>
              </ul>
            </div>
          </div>

          <div class="rowTab">
            <div class="labelTab">
              <label id="text-label" for="text"
                >Any complaint or feedback?</label
              >
            </div>
            <div class="inputTab">
              <textarea
                id="comments"
                class="input-field"
                type="text"
                placeholder="Just fill your thougths here.."
              ></textarea>
            </div>
          </div>
          <button id="submit" type="submit">Submit</button>
        </form>
      </div>
    </body>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
body {
  font-family: Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue',
    sans-serif;
  text-align: center;
  background-color: lightcoral;
}

#form-outer {
  background-color: whitesmoke;
  margin: 0 auto;
  padding: 15px;
  border-radius: 10px;
  width: 75%;
  max-width: 900px;
}

.labelTab {
  display: inline-block;
  text-align: right;
  width: 40%;
  padding: 5px;
  vertical-align: top;
  margin-top: 10px;
}

.inputTab {
  display: inline-block;
  text-align: left;
  width: 48%;
  vertical-align: middle;
}

.input-field {
  height: 20px;
  width: 70%;
  padding: 5px;
  margin: 8px;
  border: 1px solid rgba(240, 128, 128, 0.5);
  border-radius: 5px;
}

.dropdown {
  height: 33px;
  width: 75%;
  padding: 5px;
  margin: 10px;
  margin-top: 15px;
  border: 1px solid rgba(240, 128, 128, 0.5);
  border-radius: 5px;
}

.radio,
.checkbox {
  position: relative;
  left: -15%;
  margin-left: 10px;
  display: block;
  padding-bottom: 10px;
}
#submit {
  background-color: rgba(240, 128, 128, 0.75);
  border-radius: 5px;
  color: white;
  font-size: 1em;
  height: 40px;
  width: 120px;
  margin: 10px;
  border: 0px solid;
}

textarea {
  height: 50px;
  resize: vertical;
}

@media screen and (max-width: 520px) {
  .labelTab {
    width: 100%;
    text-align: left;
  }
  .inputTab {
    width: 80%;
    float: left;
  }
  .input-field {
    width: 100%;
  }
  select {
    width: 100%;
  }
}
</style>
