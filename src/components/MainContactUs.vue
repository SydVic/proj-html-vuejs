<template>
  <section class="contact-us">
    <div class="container-general">
      <div class="row">
        <div class="col-lg-8">
          <div class="form-wrapper">
            <div class="form-text">
              <h3 class="title-small">send a message</h3>
              <h2 class="title">
                <span class="title-normal">Get in </span>
                <span class="title-highlighted txt-brand">Touch</span>
              </h2>
              <p class="paragraph">We will respond to your message as soon as possible.</p>
              <form action="">
                <input type="text" class="" placeholder="Name">
                <input type="email" class="" placeholder="Email">
                <input type="text" class="" placeholder="Phone">
                <select name="" id="">
                  <option value="">More Info</option>
                </select>
                <input type="text" class="" placeholder="Message">
              </form>
            </div>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="contacts-wrapper"></div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "MainContactUs",
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

section.contact-us {
  padding: 8rem 0;

  .paragraph {
    color: $shark;
  }
}
</style>