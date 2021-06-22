<template>
  <div>
    <q-list v-for="card in cardss" :key="card.head">
      <q-item class="flex-center">
        <q-card class="shadow-12 col-9 cardStylle">
          <q-card-section class="text-h3 text-center">
            {{ card.head }}
          </q-card-section>
          <q-card-section class="row">
            <div class="q-pa-md">
              <div class="flex-center flex">
                <q-img :src="card.image" width="30%" />
              </div>
              <div class="q-gutter-y-md q-mt-xl column">
                <div class="text-h6">
                  {{ card.statement1 }}
                </div>
                <div class="text-subtitle1">
                  {{ card.content1 }}
                </div>
                <div class="text-h6">
                  {{ card.statement2 }}
                </div>
                <div class="text-subtitle1">
                  {{ card.content2 }}
                </div>
              </div>
            </div>
          </q-card-section>
        </q-card>
      </q-item>
    </q-list>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cardss: [
        {
          head: "Business Performance",
          image: "http://quantumworld.in/wp-content/uploads/2016/11/15-2.jpg",
          statement1: "How to Drive BYOD in Your Organization",
          content1:
            "BYOD is running ahead of organizational thinking and regulatory policy. So, how can companies ensure they're driving the change rather than trying to catch up?",
          statement2:
            "The Architect – Finding the Right Mix: On-Premise and Cloud-Based Computing",
          content2:
            "Charging for IT on the basis of usage, like electricity is billed, has always been an attractive proposition. Some think that utility computing could commoditize IT such that it ceases to play a strategic business role. Businesses would differentiate only on processes and business models.",
        },
        {
          head: "Digital Experiences",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/420xNxinfogr-multi-platform-digital-experience.jpg.pagespeed.ic_.hWEtqfHA4D.jpg",
          statement1: "Digitizing the Publishing Enterprise",
          content1:
            "Digitizing the Publishing Enterprise For the publishing industry, “being digital” is no longer an add-on to the core physical publishing business, a “nice to have” element on the periphery. Publishers will need to reengineer and reinvent their businesses and need new systems to manage the new digital enterprise.",
          statement2: "Digitization: The Way Forward for Automotive Companies",
          content2:
            "Digitization: The Way Forward for Automotive Companies Automotive companies can respond to market challenges and address the emerging trends by implementing a phased digital business strategy, choosing the right digital technology portfolio across the value chain and aligning these with the core competencies and the chosen strategies of the organization",
        },
        {
          head: "Customers and Markets",
          image: "http://quantumworld.in/wp-content/uploads/2016/11/15-3.jpg",
          statement1:
            "A Dozen Ways Insurers Can Leverage Big Data for Business Value",
          content1:
            "With the proliferation of social media channels, insurers are receiving voluminous customer data and finding it challenging to process and generate benefits from it. They can channel this overwhelming data to reap benefits like increased productivity, improved competitive advantage and enhanced customer experience by analyzing the data effectively.",
          statement2:
            "Clear Visibility: The Financial Insight to Drive Better Outcomes",
          content2:
            "Real-time, forward-looking financial insight and analysis are “make or break” for enterprises today. CFOs who rise to this challenge will achieve greater visibility across their enterprises and using that visibility to improve strategic decision-making, build more agile operations, giving their organizations an edge over their competitors.",
        },
      ],
    };
  },
};
</script>

<style>
.cardStylle {
  background: radial-gradient(
    circle,
    rgba(108, 204, 207, 1) 0%,
    rgba(169, 199, 235, 1) 91%
  );
}
</style>
