<template>
    <div id="contact" class="container">
        <div class="wrapper">
            <div class="form">
                <h2>Contact Form</h2>
                <p>Feel free to contact me if you have any questions and/or concerns. If you prefer communication via a platform other than email, leave your contact details below and I'll get back to you.</p>
                <form action="https://formspree.io/f/mjvzozbl" method="POST">
                    <p>
                        <input id="name" name="firstname" class="form-input" type="text" placeholder="Your name" required>
                        <small class="name-error"></small>
                    </p>
                    <p>
                        <input id="surname" name="lastname" class="form-input" type="text" placeholder="Your last name" required>
                        <small class="name-error"></small>
                    </p>
                    <p> <input id="email" name="email" class="form-input" type="email" placeholder="Your email" required>
                    <small class="name-error"></small>
                    </p>
                    
                    <p> <input id="company" name="company" class="form-input" type="text" placeholder="Company/Institution Name">
                      <small></small>
                    </p>
                    <p class="full-width">
                        <textarea minlength="10" id="message" name="message" cols="20" rows="9" placeholder="Type message here..." required></textarea>
                    </p>
                    <p class="full-width">
                        <b><input type="submit" class="submit-btn" value="submit" onclick="checkValidations()"></b>
                    </p>
                </form>
            </div>
        </div>
    </div>
</template>

<script>

    export default {
        name
        
    }

</script>

<style scoped>
body {
  padding: 1rem;
  color: #030701;
  font-family: 'Roboto', sans-serif;
}

.container {
  max-width: 1170px;
  margin-left: auto;
  margin-right: auto;
  padding: 1em;
}

div.form {
  background-color: #ffffff7e;
  border-radius: 15px;
}
.contact-wrapper {
  margin: auto 0;
}

.submit-btn {
  float: left;
}
@media (min-width: 600px) {
  .contain {
    padding: 0;
  }
}

h3,
ul {
  margin: 0;
}

h3 {
  margin-bottom: 1rem;
}

.form-input:focus,
textarea:focus{
  outline: 1.5px solid #76d337;
}

.form-input,
textarea {
  width: 100%;
  border: 1px solid #bdbdbd;
  border-radius: 5px;
}

.wrapper > * {
  padding: 1em;
}
@media (min-width: 700px) {
  .wrapper {
    display: grid;
    grid-template-columns: 2fr 1fr;
  }
  .wrapper > * {
    padding: 2em 2em;
  }
}

li
{
   display: inline-block;
   float:left;
}

ul {
    margin: 0;
    padding: 0;
    display: inline-block;
}

a{
    text-decoration: none;
    color: #f2f2f2;
    padding: 1rem;
    display: block;
    text-shadow: 0px 1px 1px #030701;
}

.contacts {
  color: #030701;
}

.form {
  background:  #f7ffd7;
}

form {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 20px;
}
form label {
  display: block;
}
form p {
  margin: 0;
}

.full-width {
  grid-column: 1 / 3;
}

button,
.submit-btn,
.form-input,
textarea {
  padding: 1em;
}

button, .submit-btn {
  background: transparent;
  border: 1px solid #030701;
  color: #030701;
  border-radius: 15px;
  padding: 5px 20px;
  text-transform: uppercase;
}
button:hover, .submit-btn:hover,
button:focus , .submit-btn:focus{
  background: #030701;
  outline: 0;
  color: #f7ffd7;
}
.error {
  color: #76d337;
}
</style>