<template>
  <div class="container info-container">
    <b-row class="mt-5 mb-3">
      <b-col sm="12" md="6" class="map">
        <div style="width: 100%;position: relative;">
          <iframe
            width="100%"
            height="600"
            src="https://maps.google.com/maps?width=400&amp;height=600&amp;hl=en&amp;q=9%20rue%20francis%20davso%2C%2013001%20marseille+(test)&amp;ie=UTF8&amp;t=&amp;z=15&amp;iwloc=B&amp;output=embed"
            frameborder="0"
            scrolling="no"
            marginheight="0"
            marginwidth="0"
          >
          </iframe>
          <div
            style="position: absolute;width: 80%;bottom: 10px;left: 0;right: 0;margin-left: auto;margin-right: auto;color: #000;text-align: center;"
          >
            <small style="line-height: 1.8;font-size: 2px;background: #fff;">
              Powered by
              <a href="http://www.googlemapsgenerator.com/ja/">
                googlemapsgen (ja)
              </a>
              &
              <a href="http://brightononline.ca/fr/">
                custommapprints (fr)
              </a>
            </small>
          </div>
          <style>
            #gmap_canvas img {
              max-width: none !important;
              background: none !important;
            }
          </style>
        </div>
        <br />
      </b-col>
      <b-col sm="12" md="6" class="horaires">
        <h3>Consultations</h3>
        <hr />
        <br />
        <h4>Lundi</h4>
        <p>Matin : 9h00 -12h00 Après-midi: 14h00 19h00</p>
        <h4>Mardi</h4>
        <p>Matin : 9h00 -12h00 Après-midi: 14h00 19h00</p>
        <h4>Mercredi</h4>
        <p>Matin : 9h00 -12h00 Après-midi: 14h00 19h00</p>
        <h4>Jeudi</h4>
        <p>Matin : 9h00 -12h00 Après-midi: <strong>Fermé</strong></p>
        <h4>Vendredi</h4>
        <p>Matin : 9h00 -12h00 Après-midi: 14h00 19h00</p>
        <br />
        <hr />
        <h4>Nos consultations sont exclusivement sur rendez-vous</h4>
      </b-col>
    </b-row>
  </div>
</template>

<style scoped lang="scss">
$border-custom: #c9c9c9;
.info-container {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 70vh;
  text-align: center;
  p {
    font-family: 'Montserrat', sans-serif;
  }
}
</style>
