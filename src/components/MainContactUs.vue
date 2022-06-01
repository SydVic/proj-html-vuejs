<template>
  <section class="contact-us">
    <div class="container-general">
      <div class="row">
        <div class="col-lg-7">
          <div class="form-wrapper">
            <div class="form-text">
              <h3 class="title-small">send a message</h3>
              <h2 class="title">
                <span class="title-normal">Get in </span>
                <span class="title-highlighted txt-brand">Touch</span>
              </h2>
              <p class="paragraph">We will respond to your message as soon as possible.</p>
              <!-- FORM -->
              <form class="contact-us" action="">
                <input type="text" class="input-name" placeholder="Name">
                <input type="email" class="" placeholder="Email">
                <input type="text" class="" placeholder="Phone">
                <select class="options-select" name="" id="">
                  <option value="">More Info</option>
                </select>
                <textarea class="leave-message" placeholder="Message"></textarea>
              </form>
              <!-- /FORM -->
              <div class="btn">
                <div class="btn-primary">send</div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4 col-lg-offset-1">
          <div class="contacts-wrapper">col 4</div>
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

  .contact-us {
    width: 100%;
    margin-top: 3.5rem;

    input[type=text],
    input[type=email],
    select,
    textarea {
      padding: .9rem .7rem;
      background-color: $gray-nurse;
      border-color: transparent;
      border-radius: 5px;
      color: #8175a1;
      font-size: 1rem;
      margin-bottom: 1rem;

      &::placeholder {
        font-size: 1rem;
        color: #8175a1;
      }
    }

    input[type=text] {
      width: calc(50% - .5rem);
      margin-right: .5rem;
    }

    input[type=email] {
      width: calc(50% - .5rem);
      margin-left: .5rem;
    }

    select.options-select {
      width: calc(50% - .5rem);
      margin-left: .5rem;
    }

    textarea.leave-message {
      font-family: "Lato", sans-serif;
      width: 100%;
      min-height: 150px;
      resize: none;
    }
  }

  .btn {
    margin-top: .5rem;
  }
}
</style>