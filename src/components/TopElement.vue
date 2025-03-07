<script setup></script>

<template>
  <article class="wrapper">
    <section id="hero">
      <section id="hero__content">
        <h4>Branding | Imaging</h4>
        <h1>My awesome portfolio</h1>
        <p>
          This is a template Figma file. For more, look up the template at the
          publisher's profile "Anima"
          <a href="https://www.figma.com/community/file/1184894959333450190"
            >here</a
          >.<br /><br />
          This template is only for test purpose and therefore does not have
          full functionality of the form element below and the menu links, with
          the exception of the GitHub link.
        </p>
      </section>
      <img
        id="hero__image"
        src="../assets/topElementImage.png"
        alt="Top Element Image"
      />
    </section>
  </article>
</template>

<style scope>
#hero {
  display: block;

  #hero__image {
    width: 300px;
  }
}
h1 {
  font-size: var(--h1-size);
  line-height: 1.1;
  font-weight: 600;
  margin-block: 2rem;
}
h4 {
  font-size: var(--h4-size);
  font-weight: 500;
}
p {
  font-size: var(--text-size);
}

/** tablet and desktop breakpoint for hero component */
@media (min-width: 700px) {
  #hero {
    display: flex;
    align-items: center;
  }
}
</style>
