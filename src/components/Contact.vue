<script setup></script>

<template>
  <article class="wrapper" id="contact__card">
    <div class="line"></div>
    <section class="contact">
      <section class="contact__description">
        <h3>Let's work together</h3>
        <p>
          This is a template Figma file. Reach out to me for collaborations and
          project feedbacks. For updates on upcoming projects, write me an email
          to get updates.
        </p>
      </section>
      <section class="contact__form">
        <form action="">
          <fieldset class="form">
            <input type="text" class="text-field" placeholder="Name" />
            <input type="text" class="text-field" placeholder="Email" />
            <textarea
              rows="5"
              cols=""
              type="textarea"
              class="text-field"
              placeholder="Type your message here"
            ></textarea>
          </fieldset>
          <input type="button" class="button" value="Submit" />
        </form>
      </section>
    </section>
  </article>
</template>

<style scoped>
@media (min-width: 700px) {
  #contact__card {
    margin-top: 1rem;
  }
  .contact {
    display: flex;
    justify-content: space-evenly;
  }
  .contact__description {
    width: 50%;
  }
  .contact__form {
    width: 50%;
    margin-left: 3rem;
  }
  h3 {
    display: block;
    margin: 0;
  }
}
.line {
  width: min(67.5rem, calc(100% - 6.25rem));
  height: 0;
  border: solid #ffd285;
  border-width: thin;
  margin-inline: auto;
  margin-top: 2rem;
  margin-bottom: 2rem;
}
.form {
  display: grid;
  border: none;
  padding: 0px;
}
input {
  display: block;
  font-size: var(--text-size);
}
input.text-field,
.text-field {
  margin-top: 0;
  margin-bottom: 0.5rem;
  border: none;
  border-radius: 3px;
  background-color: #f3f3f3;
  min-height: 2rem;
}
input.button {
  width: 8.5rem;
  height: 3rem;
  display: flex;
  margin-inline: auto;
}
textarea {
  resize: none;
}
.button {
  background-color: #2d2d2d;
  color: #ffffff;
  font-size: var(--h4-size);
  font-weight: 100;
}
h3 {
  font-size: var(--h3-size);
}
p {
  font-size: var(--text-size);
}
</style>
