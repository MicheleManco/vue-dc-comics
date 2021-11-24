<template>
  <div id="banner-blue">
      <ul id="products">
          <li v-for="prodotto,i in prodotti" :key="i">
              <img :src="prodotto.image" alt="">
              {{prodotto.text}}
            </li>
      </ul>
      <div class="banner">
          <div class="separatore-footer">
            <div>   
              <h3>DC COMICS</h3>
              <ul>
                  <li>Characters</li>
                  <li>Comics</li>
                  <li>Movies</li>
                  <li>TV</li>
                  <li>Games</li>
                  <li>Videos</li>
                  <li>News</li>
              </ul>
              <h3>SHOP</h3>
              <ul>
                  <li>Shop DC</li>
                  <li>Shop DC Collectibles</li>
              </ul>
            </div>

            <div>
                <h3>DC</h3>
                <ul>
                    <li>Terms of Use</li>
                    <li>Privacy Policy (New)</li>
                    <li>ad choices</li>
                    <li>advertising</li>
                    <li>jobs</li>
                    <li>subscriptions</li>
                    <li>talent workshops</li>
                    <li>CPSC certificates</li>
                    <li>Rating</li>
                    <li>shop help</li>
                    <li>contact us </li>
                </ul>
            </div>

            <div>
                <h3>SITES</h3>
                <ul>
                    <li>DC</li>
                    <li>MAD magazine</li>
                    <li>DC kids</li>
                    <li>DC Universe</li>
                    <li>DC power Visa</li>
                </ul>
            </div>
          </div>
          <div>
              <img src="../assets/img/dc-logo-bg.png" alt="">
          </div>
      </div>
      <div class="gray">

      </div>
  </div>
</template>

<script>
export default {
  name: 'Footer',
    data() {
        return{
            prodotti:[
                {
                text: "DIGITAL COMICS",
                image: "../assets/img/buy-comics-digital-comics.png"   
                },
                {
                text: "DC MERCHANDISE",
                image: "../assets/img/buy-comics-merchandise.png"   
                },
                {
                text: "SUBSCRIPTION",
                image: "../assets/img/buy-comics-subscriptions.png"   
                },
                {
                text: "COMIC SHOP LOCATOR",
                image: "../assets/img/buy-comics-shop-locator.png"   
                },
                {
                text: "DC POWER VISA",
                image: "../assets/img/buy-dc-power-visa.png"   
                }
            ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#banner-blue {
    background-color: rgb(0, 110, 255);
    color: white;
    #products {
        width: 80%;
        margin: 0 auto;
        list-style: none;
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100px;
    }
    .banner {
        background-image: url("../assets/img/footer-bg.jpg");
        display: flex;
        justify-content: space-between;
        .separatore-footer {
            display: flex;
            width: 80%;
            margin: 0 auto;
        }
    }
}

</style>