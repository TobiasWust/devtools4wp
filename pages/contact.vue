<template>
  <div class="contactpage">
    <h1 class="title">
      Kontakt
    </h1>
    <hr>
      <form name="contact" action="/success/" method="POST" netlify>
        <input type="hidden" name="form-name" value="contact" />
        <label>Email*<input name="email" id="email" placeholder="Email" type="email" required /></label> 
        <label>Name<input name="name" id="name" placeholder="Name" /></label>               
        <label>Nachricht<textarea class="form-field" name="message" id="message" rows="6" placeholder="Deine Nachricht"></textarea></label>                     
        <label class="container">Ich akzeptiere die <nuxt-link to="/privacy/">Datenschutzbestimmungen</nuxt-link>*
          <input name="privacy" id="privacy" type="checkbox" required />
          <span class="checkmark"></span>
        </label>
        <input class="form-button" type="submit" value="Senden" />
      </form>
      <span style="font-size:0.7em;">* Kennzeichnet Pflichtfelder</span>
    </div>
</template>

<script>
export default {
  head: {
    title: "Kontakt",
    meta: [
      {
        hid: "description",
        name: "description",
        content:
          "Hi, ich bin Tobias Wust. Ich bin ein reisender Fullstack Entwickler. Nimm doch Kontakt mit mir auf!"
      }
    ]
  }
};
</script>

<style scoped>
form {
  font-weight: bold;
}

.container {
  display: block;
  position: relative;
  padding-left: 35px;
  margin-bottom: 12px;
  cursor: pointer;
  user-select: none;
}

/* Hide the browser's default checkbox */
.container input {
  position: absolute;
  opacity: 0;
  cursor: pointer;
}

/* Create a custom checkbox */
.checkmark {
  position: absolute;
  top: 0;
  left: 0;
  height: 25px;
  width: 25px;
  background-color: #999;
}

/* On mouse-over, add a grey background color */
.container:hover input ~ .checkmark {
  background-color: #3dba6a;
}

/* When the checkbox is checked, add a blue background */
.container input:checked ~ .checkmark {
  background-color: #3dba6a;
}

/* Create the checkmark/indicator (hidden when not checked) */
.checkmark:after {
  content: "";
  position: absolute;
  display: none;
}

/* Show the checkmark when checked */
.container input:checked ~ .checkmark:after {
  display: block;
}

/* Style the checkmark/indicator */
.container .checkmark:after {
  left: 10px;
  top: 6px;
  width: 5px;
  height: 10px;
  border: solid white;
  border-width: 0 3px 3px 0;
  -webkit-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  transform: rotate(45deg);
}

input,
textarea {
  width: 100%;
  border: none;
  padding: 10px;
}

.form-button {
  color: white;
  background-color: #f68714;
  border: none;
  width: 200px;
  height: 40px;
  transition: all 1s ease;
}

.form-button:hover {
  background-color: #3dba6a;
}
</style>