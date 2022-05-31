<template>
  <!-- SECTION WHO WE ARE -->
  <section class="who-we-are">
    <div class="container-small">
      <div class="row">
        <div class="col-lg-8">
          <div class="text-section">
            <h3 class="title-small">who we are</h3>
            <h2 class="title">
              <span class="title-highlighted txt-brand">
                <i class="far fa-gem"></i> 
                Excellence 
              </span>
              <span class="title-normal">in Transport</span>
            </h2>
            <div class="text-wrapper">
              <p class="paragraph">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam sunt necessitatibus neque rerum vero veritatis accusamus blanditiis maxime architecto repudiandae error qui, quae, aliquam enim dolor consequuntur explicabo, placeat id.</p>
              <p class="paragraph">Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum, quis dolorum quasi consectetur repellendus quod, sed, id ratione quia obcaecati nam atque soluta eius sint enim! Esse alias itaque qui.</p>
              <p class="paragraph italic">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod, ipsa a, earum odit facilis deserunt architecto, aliquid tempora autem qui aut quam delectus neque eius accusamus magni consequatur rerum voluptatum.</p>
              <p class="paragraph">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
              <ul>
                <li>Lorem ipsum dolor sit amet</li>
                <li>Consectetur adipisicing elit</li>
                <li>Integer molestie lorem at massa</li>
                <li>Facilisis in pretium nisl aliquet</li>
                <li>Dapibus hendrerit mauris curabitur</li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="vehicle-types">
            <h2>Vehicle Types</h2>
            <div class="vehicle-type">
              <div class="vehicle-img">
                <img src="../assets/img/truck-1.png" alt="">
              </div>
              <div class="vehicle-specs">
                <h3>Light</h3>
                <p>Max Weight 1200kg</p>
              </div>
            </div>
            <div class="vehicle-type">
              <div class="vehicle-img">
                <img src="../assets/img/truck-1.png" alt="">
              </div>
              <div class="vehicle-specs">
                <h3>Medium</h3>
                <p>Max Weight 6000kg</p>
              </div>
            </div>
            <div class="vehicle-type">
              <div class="vehicle-img">
                <img src="../assets/img/truck-1.png" alt="">
              </div>
              <div class="vehicle-specs">
                <h3>Heavy</h3>
                <p>Max Weight 24000kg</p>
              </div>
            </div>
          </div>
          <div class="certifications">
            <h2>Certifications</h2>
            <div class="certifications-img">
              <img src="../assets/img/certificate.png" alt="">
            </div>
            <div class="certifications-img">
              <img src="../assets/img/certificate.png" alt="">
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- /SECTION WHO WE ARE -->
</template>

<script>
export default {
  name: "MainWhoWeAre",
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

section.who-we-are {
  padding: 8rem 0;

  .text-section {
    padding-right: 2rem;
  
    i {
      padding-left: 1rem;
    }
    
    .title-normal {
      padding-left: .5rem;
    }
  
    .text-wrapper {
      color: $shark;
  
      .italic {
        border-left: 5px solid $brand-primary-shadow;
        padding: 1rem 5rem 1rem 1.5rem;
        font-style: italic;
      }
  
      ul {
      list-style: disc;
      margin-left: 1rem;
  
        li {
          margin-bottom: .8rem;
        }
      }
    }
  }
  
  .vehicle-types {
    margin-bottom: 2.5rem;

    h2 {
      margin-bottom: 1.8rem;
    }

    .vehicle-type {
      width: 100%;
      display: flex;
      align-items: center;
      padding:  1rem 0 1rem 0;

      &:not(:last-child) {
        border-bottom: 1px solid black;
      }
    
      .vehicle-img {
        width: 30%;
        background-color: rgba(22, 146, 142, .4);
        padding: .3rem .3rem;
        border-radius: 5px;
      }

      .vehicle-specs {
        padding: 0 1.5rem;

        h3 {
          font-size: 1.5rem;
          margin-bottom: .5rem;
        }
      }
    }
  }

  .certifications {

    h2 {
      margin-bottom: 1rem;
    }
    .certifications-img {
      width: 50%;
      display: inline-block;
      padding: 1rem;
    }
  }
}
</style>