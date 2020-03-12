<template>
  <div class="about">
    <h1>Try to use Vue.js</h1>
    <br />
    <div>
      <b-container>
        <b-card no-body class="w-100" align="center">
          <b-tabs card>
            <b-tab title="Media" active>
              <b-card>
                <b-media no-body>
                  <b-media-aside vertical-align="center">
                    <b-img
                      src="https://picsum.photos/200/300"
                      width="128"
                      height="256"
                      alt="ini gambar"
                    ></b-img>
                  </b-media-aside>

                  <b-media-body class="ml-3">
                    <h5 class="mt-0">Media</h5>
                    <p>
                      Ini adalah contoh dari tampilan media. media adalah suatu
                      alat perantara atau pengantar yang berfungsi untuk
                      menyalurkan pesan atau informasi dari suatu sumber kepada
                      penerima pesan. Pendapat lain mengatakan arti media adalah
                      segala bentuk saluran yang dapat digunakan untuk
                      menyampaikan informasi atau pesan. Dengan kata lain, media
                      dapat didefinisikan sebagai sarana untuk menyampaikan
                      suatu pesan. Secara etimologi kata “media” berasal dari
                      bahasa Latin, yaitu “medius” yang artinya “tengah,
                      perantara atau pengantar”. Istilah “media” pada umumnya
                      merujuk pada sesuatu yang dijadikan sebagai wadah, alat,
                      atau sarana untuk melakukan komunikasi.
                    </p>

                    <b-media>
                      <template v-slot:aside>
                        <b-img
                          src="https://picsum.photos/seed/picsum/200/300"
                          width="64"
                          alt="placeholder"
                        ></b-img>
                      </template>
                      <h5 class="mt-0">Jenis Media</h5>
                      <p align="center">
                        &#9679; Audio <br />
                        &#9679; Visual <br />
                        &#9679; Audio Visual <br />
                      </p>
                    </b-media>
                  </b-media-body>
                </b-media>
              </b-card>
            </b-tab>
            <b-tab title="Images">
              <b-card-text>
                <b-container fluid class="p-4 bg-dark">
                  <b-row>
                    <b-col>
                      <b-img
                        thumbnail
                        fluid
                        src="https://picsum.photos/250/250/?image=54"
                        alt="Image 1"
                      ></b-img>
                    </b-col>
                    <b-col>
                      <b-img
                        thumbnail
                        fluid
                        src="https://picsum.photos/250/250/?image=58"
                        alt="Image 2"
                      ></b-img>
                    </b-col>
                    <b-col>
                      <b-img
                        thumbnail
                        fluid
                        src="https://picsum.photos/250/250/?image=59"
                        alt="Image 3"
                      ></b-img>
                    </b-col>
                  </b-row>
                </b-container>
              </b-card-text>
            </b-tab>
          </b-tabs>
        </b-card>
      </b-container>
    </div>
  </div>
</template>
