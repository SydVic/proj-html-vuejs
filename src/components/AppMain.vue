<template>
  <section class="main">
    <div class="container-small">
      <div class="row">
        <div class="col-lg-8">
          <h3 class="subtitle">who we are</h3>
          <h2>
            <span class="title-highlighted">
              <i class="far fa-gem"></i> 
              Excellence 
            </span>
            <span class="title-normal">in Transport</span>
          </h2>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam sunt necessitatibus neque rerum vero veritatis accusamus blanditiis maxime architecto repudiandae error qui, quae, aliquam enim dolor consequuntur explicabo, placeat id.</p>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum, quis dolorum quasi consectetur repellendus quod, sed, id ratione quia obcaecati nam atque soluta eius sint enim! Esse alias itaque qui.</p>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod, ipsa a, earum odit facilis deserunt architecto, aliquid tempora autem qui aut quam delectus neque eius accusamus magni consequatur rerum voluptatum.</p>
          <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
          <ul>
            <li>Lorem</li>
            <li>Lorem</li>
            <li>Lorem</li>
            <li>Lorem</li>
            <li>Lorem</li>
          </ul>
        </div>
        <div class="col-lg-4">
          <h3>Vehicle Types</h3>
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
              <h3>Light</h3>
              <p>Max Weight 1200kg</p>
            </div>
          </div>
          <div class="vehicle-type">
            <div class="vehicle-img">
              <img src="../assets/img/truck-1.png" alt="">
            </div>
            <div class="vehicle-specs">
              <h3>Light</h3>
              <p>Max Weight 1200kg</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppMain",
}
</script>

<style lang="scss" scoped>
h2 {
  font-size: 3rem;
}

.vehicle-type {
  width: 100%;
  display: flex;
  align-items: center;
  border-bottom: 1px solid black;
  padding:  1rem 0 1rem 0;

  .vehicle-img {
    width: 30%;
    background-color: rgba(22, 146, 142, .4);
    padding: .3rem .3rem;
    border-radius: 5px;

    img {
      width: 100%;
    }
  }
}

ul {
  list-style: disc;
  margin-left: 1rem;
}
</style>