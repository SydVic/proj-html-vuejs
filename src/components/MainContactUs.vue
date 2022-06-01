<template>
  <section class="contact-us">
    <!-- CONTAINER WIDTH60% -->
    <div class="container-general">
      <!-- ROW -->
      <div class="row">
        <!-- COL-7 -->
        <div class="col-lg-7">
          <!-- FORM SECTION WRAPPER -->
          <div class="form-wrapper">
            <!-- FORM TITLE AND TEXT -->
            <div class="form-text">
              <h3 class="title-small">send a message</h3>
              <h2 class="title">
                <span class="title-normal">Get in </span>
                <span class="title-highlighted txt-brand">Touch</span>
              </h2>
              <p class="paragraph">We will respond to your message as soon as possible.</p>
            </div>
            <!-- /FORM TITLE AND TEXT -->

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
          <!-- /FORM SECTION WRAPPER -->
        </div>
        <!-- /COL-7 -->

        <!-- COL-4 -->
        <div class="col-lg-4 col-lg-offset-1">
          <div class="contacts-wrapper">
            <h2>Example Inc.</h2>
            <p class="paragraph">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
            <p class="paragraph">Praesent diam lacus, dapibus sed imperdiet consectetur.</p>
            <ul class="company-contacts">
              <li>
                <span class="icon-wrapper">
                  <i class="fas fa-phone-alt"></i>
                </span>
                <span class="text-wrapper">
                  {{ companyObject.phone }}
                </span>
              </li>
              <li>
                <span class="icon-wrapper">
                  <i class="fas fa-envelope"></i>
                </span>
                <span class="text-wrapper">
                  {{ companyObject.eMail }}
                </span>
              </li>
              <li>
                <span class="icon-wrapper">
                  <i class="fas fa-map-marker-alt"></i>
                </span>
                <span class="text-wrapper">
                  {{ companyObject.location }}
                </span>
              </li>
            </ul>
            <div class="btn">
              <a class="btn-secondary" href="">view map</a>
            </div>
          </div>
        </div>
        <!-- /COL-4 -->
      </div>
      <!-- /ROW -->
    </div>
    <!-- /CONTAINER WIDTH60% -->
  </section>
</template>

<script>
export default {
  name: "MainContactUs",
  props: {
    companyObject: Object,
  }
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

  ul.company-contacts {
    color: $brand-primary;

    li {
      margin-bottom: 1.5rem;

      span {
        display: inline-block;
        font-size: 1.2rem;
      }

      span.icon-wrapper {
        background-color: $brand-primary-shadow;
        width: 45px;
        height: 45px;
        text-align: center;
        vertical-align: middle;
        line-height: 45px;
        border-radius: 50%;
        margin-right: 1rem;

        i {
          vertical-align: middle;
        }
      }
    }
  }

  .btn-secondary {
    color: $brand-primary;

    &:hover {
      color: $silver-sand;
    }
  }
}
</style>