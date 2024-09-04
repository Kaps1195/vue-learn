<template>
  <div class="contact-us">
    <h1>Contact Us</h1>
  </div>
  <div>
    <h4>Fill out the form and we'll be in touch soon!</h4>
    <h3>How can we help you?</h3>
    <form action="/submit-form" method="POST">
      <div class="form-group">
        <input placeholder="First Name" type="text" required />
      </div>
      <div class="form-group">
        <input placeholder="Last Name" type="text" required />
      </div>
      <div class="form-group">
        <input placeholder="Your email" type="email" required />
      </div>
      <div class="form-group">
        <textarea placeholder="Your message" required></textarea>
      </div>
      <button type="submit">Send Message</button>
    </form>
  </div>
</template>

<style>
.contact-us {
  display: flex;
  justify-content: center;
  background-color: blueviolet;
  margin-top: 50px;
  padding: 50px;
}

h1 {
  font-family: 'Poppins', Sans-serif;
  font-weight: 500;
  color: white;
}
.form-group {
  margin-bottom: 15px;
}

input {
  width: 50%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
}

textarea {
  width: 80%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
}

button {
  background-color: #007bff;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

button:hover {
  background-color: #0056b3;
}

@media (min-width: 1024px) {
}
</style>
