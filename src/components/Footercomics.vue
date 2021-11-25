<template>
<div>
    
<div id="banner-blue">
      <ul id="products">
          <li v-for="(prodotto,i) in prodotti" :key="i">
              <img src="require(`./assets/img/${prodotto.image}`)">
              {{prodotto.text}}
            </li>
      </ul>
    </div>


      <div class="banner">
          <div id="contenitore-footer">
            <div class="links-footer">
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

          <div id="dc-logo">
              <img src="../assets/img/dc-logo-bg.png" alt="">
          </div>
          </div>
          
      </div>
      <div class="gray">
          <div id="container-bottom">
              <div id="btn">
                  SIGN-UP NOW!
              </div>
              <div id="social-btns">
                  <div id="follow-blu">FOLLOW US</div>
                  <div><img src="../assets/img/footer-facebook.png" alt=""></div>
                  <div><img src="../assets/img/footer-twitter.png" alt=""></div>
                  <div><img src="../assets/img/footer-youtube.png" alt=""></div>
                  <div><img src="../assets/img/footer-pinterest.png" alt=""></div>
                  <div><img src="../assets/img/footer-periscope.png" alt=""></div>
              </div>
          </div>
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
                image: "buy-comics-digital-comics.png"   
                },
                {
                text: "DC MERCHANDISE",
                image: "buy-comics-merchandise.png"   
                },
                {
                text: "SUBSCRIPTION",
                image: "buy-comics-subscriptions.png"   
                },
                {
                text: "COMIC SHOP LOCATOR",
                image: "buy-comics-shop-locator.png"   
                },
                {
                text: "DC POWER VISA",
                image: "buy-dc-power-visa.png"   
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
}
.banner {
    background-image: url("../assets/img/footer-bg.jpg");
    height: 400px;
    display: flex;
    background-repeat: no-repeat;
    background-size: cover;
    #contenitore-footer {
        width: 80%;
        margin: 0 auto;
        display: flex;
        justify-content: center;
        align-items: center;
        color: white;

        .links-footer {
            display: flex;
            width: 80%;
            ul{
                list-style: none;
                margin-right: 30px;
                margin-bottom: 20px;
                color: gray;
            }
        }
    }
}
.gray {
    background-color: rgb(43, 43, 43);
    height: 80px;
}
#container-bottom {
    height: 100%;
    width: 80%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
#btn {
        border: 2px solid rgb(0, 110, 255);
        padding: 10px;
        color: white;
    }
#social-btns {
    display: flex;
    align-items: center;
    div{
        margin: 10px;
    }
    #follow-blu {
        color: rgb(0, 110, 255);
    }
}

</style>