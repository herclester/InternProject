<template>
  <div>
    <div class="row homeBg flex-center q-pa-xl">
      <div class="text-h3 col-3 column">
        <div style="height: 10px; width: 100px" class="bg-blue-8"></div>
        <div class="text-h3">
          Quantum World is the pioneer of Engineering Manpower Outsourcing
        </div>
      </div>
      <div class="col-3">
        <q-img src="home_content.png" width="90%" />
      </div>
    </div>
    <div class="row flex-center">
      <div v-for="card in cardData" :key="card.head" class="q-pa-md">
        <q-card class="shadow-12 cardStyle row">
          <q-card-section class="text-center">
            <h4>
              {{ card.head }}
            </h4>
          </q-card-section>
          <q-card-section class="text-center text-subtitle1">
            {{ card.data }}
          </q-card-section>
        </q-card>
      </div>
    </div>
    <div class="q-pa-xl styleExtra">
      <div class="column">
        <div style="height: 10px; width: 300px" class="bg-blue-8"></div>
        <div class="text-h2 text-left">
          Quantum World <br />is a leading consulting and services company<br />
          in India (specially in Noida & Lucknow)
        </div>
      </div>
      <div class="row q-mt-xl flex-center">
        <div v-for="card in extraData" :key="card.head" class="q-pa-md">
          <q-card class="shadow-12 extraData text-center row">
            <q-card-section class="full-width text-h4 q-pa-md">
              {{ card.head }}
            </q-card-section>
            <q-card-section class="text-center text-subtitle1">
              {{ card.data }}
            </q-card-section>
          </q-card>
        </div>
      </div>
    </div>
    <div class="q-mt-md">
      <q-separator />
    </div>
    <div class="row flex-center">
      <div v-for="card in end" :key="card.head" class="text-center q-pa-md">
        <q-card class="shadow-12 endStyle text-center row">
          <q-card-section class="full-width text-h4 q-pa-md">
            {{ card.head }}
            <div class="q-mt-xl text-center text-subtitle1">
              {{ card.data }}
            </div>
          </q-card-section>
        </q-card>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cardData: [
        {
          head: "Application Development",
          data: "We as QUANTUM WORLD offers one of our best service i.e. Application Development and Maintenance Services across a variety of platforms and technologies",
        },
        {
          head: "Manpower Outsourcing",
          data: "Quantam World is the pioneer of Engineering Manpower Outsourcing services in India. We provide tailor-made solutions depending on client needs. ",
        },
        {
          head: "Career Management",
          data: "We help you respond to changing marketing conditions and emerging business opportunities by strategically mobilizing and sizing your workforce ",
        },
        {
          head: "Professional Development",
          data: "We offer a full array of resources, from online training for a small-business staff to customized programs for businesses of all sizes, including many of the Fortune 500 companies",
        },
      ],
      extraData: [
        {
          head: "Retail",
          data: "QUANTUM WORLD practice is maturing in providing consulting to global retail customers in the areas of Enterprise application service with offerings like Global ERP, Application Maintenance and Support, Digital Transformation.",
        },
        {
          head: "Outsourcing",
          data: "We provide innovative outsourcing solutions across a wide range of disciplines. The world’s leading companies turn to us for Talent Based Outsourcing, Recruitment Process Outsourcing, Managed Service Provider Solutions.",
        },
        {
          head: "Application Development",
          data: "We as QUANTUM WORLD offers one of our best service i.e. Application Development and Maintenance Services.Under this service we offer our clients the full scope of services - development, implementation on newly created or an ongoing management.",
        },
      ],
      end: [
        {
          head: "About Us",
          data: "Quantum World is a leading consulting and services company in India (specially in Noida & Lucknow) and provide a manpower solution at multinational companies. Quantum World offers wide gamut of consulting solutions customized to specific needs.",
        },
        {
          head: "Mission",
          data: "Our mission is “To mutually build a globally respected Human Capital Solutions Company that provides best-in-class human capital solutions, which will add value to client organizations”. Creating an effective link between the organization and the job seeker, at Quantum World Tech, we provide the clients with the brightest and the best candidates according to their specific requirement. Also, we provide the candidates with the opportunity of working in reputed companies by placing them according to their job interest and eligibility.",
        },
        {
          head: "Contact Us",
          data: "306, Quantum House, Kamta, Faizabad Road, Lucknow (UP), India A129, Quantum World, Sector - 63 Noida (UP), India Phone No. : +91-7800008086, 7800008096 Email : info@quantumworld.in hr@quantumworld.in",
        },
      ],
    };
  },
};
</script>

<style>
.homeBg {
  background: linear-gradient(
    0deg,
    rgba(108, 204, 207, 1) 14%,
    rgba(158, 195, 238, 1) 53%,
    rgba(52, 170, 114, 1) 100%
  );
}
.cardStyle {
  width: 300px;
  height: 400px;
  background: linear-gradient(
    0deg,
    rgba(108, 204, 207, 1) 2%,
    rgba(157, 195, 237, 1) 45%,
    rgba(69, 134, 211, 1) 87%
  );
}
.extraData {
  width: 400px;
  height: 400px;
}
.endStyle {
  width: 430px;
  height: 450px;
}
.styleExtra {
  background: linear-gradient(
    0deg,
    rgba(108, 204, 207, 1) 2%,
    rgba(253, 254, 255, 1) 25%,
    rgba(69, 134, 211, 1) 87%
  );
}
</style>
