<template>
  <div class="row">
    <q-list v-for="card in cardss" :key="card.head" class="q-pa-lg col-4">
      <q-item clickable @click="openDialog(card)">
        <q-item-section>
          <q-card class="shadow-12 text-center cardIndustry">
            <q-card-section class="text-h6">
              {{ card.head }}
            </q-card-section>
            <q-card-section>
              <q-img :src="card.image" width="50%" />
            </q-card-section>
          </q-card>
        </q-item-section>
      </q-item>
    </q-list>
    <q-dialog v-model="display">
      <q-card class="shadow-12 q-pa-lg text-subtitle1">
        <q-card-section class="text-center">
          <div class="row">
            <div class="text-h6 text-bold">{{ object.head }}</div>
            <q-space />
            <q-btn icon="close" flat @click="display = false"></q-btn>
          </div>
        </q-card-section>
        <q-card-section>
          {{ object.content }}
        </q-card-section>
        <q-card-section v-if="object.content1">
          {{ object.content1 }}
        </q-card-section>
      </q-card>
    </q-dialog>
  </div>
</template>

<script>
export default {
  methods: {
    openDialog(value) {
      this.display = true;
      Object.assign(this.object, value);
    },
  },
  data() {
    return {
      object: {},
      display: false,
      cardss: [
        {
          head: "BFSI - The Banking, Financial Services and Insurance",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/bfsi-chart.jpg",
          content:
            "We as QUANTUM WORLD have developed profound knowledge and extensive experience in the Banking, Financial Services and Insurance sector. QUANTUM WORLD has the experience and insight to help the industry's organizations, regardless of where they are in the journey to transform their internal services. By combining our extensive consulting experience and original research and analysis.",
          content1:
            "Over the past decade, we have covered the BFSI market through both published research and custom projects for end users, global in-house centers (GICs) and third-party service providers. Our BFSI outsourcing research program comprehensively covers the key dynamics of the market across IT and business processes. We as QUANTUM WORLD also provides IT staffing from support personnel to accounting, finance and business management professionals. We support all staffing needs in major segments of the BFSI industry, which includes Core Banking, Corporate banking, Wholesale Banking, Retail Banking, Payment Gateways, Mutual Funds, Accounting & Billing, Insurance and many more.",
        },
        {
          head: "Health Care",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/healthcare.png",
          content:
            "One of our clients is a leading health benefits company operating in different states of the country and serving more than a million of customers in this field. Its product portfolio includes a diversified mix of managed care products, including Preferred Provider Organizations(PPOs), Health Maintenance Organizations(HMOs) and Point-Of-Service(POS) plans. The company also offers several specialty products, including group life and disability insurance benefits, pharmacy benefit management and dental, vision and behavioral health benefits services.",
          content1:
            "As the health care industry evolves it relies more on information technology solutions. An effective health information technology strategy focuses on the tools needed to improve clinical and non-clinical health IT functions and issues, like electronic health record implementation, clinical data integration, information technology governance, confidentiality, security and strategy.",
        },
        {
          head: "Energy and Utilities",
          image: "http://quantumworld.in/wp-content/uploads/2016/11/energy.jpg",
          content:
            "The vision for tomorrow's energy landscape is Safe, Reliable & Accessible. The evolution to this state is gradual. But with information technology and consulting services as transformation enablers, enterprises can catalyze the change.",
          content1:
            "QUANTUM WORLD has been partnering with global oil and gas companies, oilfield services (OFS) providers, and other organizations to maximize the impact of their technology investments. Clients leverage our expertise to create outcomes in three key areas – business transformation, accelerating innovation, and efficient operations.One of our major electrical utility clients in the country was looking for a CRM framework to improve customer services. Its functions include distribution and supply to major customers.",
        },
        {
          head: "Telecom",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/telecom.png",
          content:
            "The QUANTUM WORLD with decades of proven experience also in the telecom industry, helps you redefine your markets with innovative solutions to become more agile, reduce fixed operations costs and introduce next generation services. Our offerings, aligned to your needs, address the challenges of the transformation programs both in network systems and business domains and help you manage and implement them with the lowest risk to derive enhanced features.",
          content1:
            "We partner with you to build and implement innovative strategies and solutions to achieve improved operational and cost efficiencie, rapid time-to-market to roll out new and innovative services, improved processes and infrastructure, reduced costs of product development and support, enhanced customer satisfaction, thereby generating an increase in customer loyalty and improved quality of services.",
        },
        {
          head: "Manufacturing",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/manufacturing.jpg",
          content:
            "The QUANTUM WORLD key executives sought out a dedicated program leader to ensure that all aspects of this highly complex, enterprise level strategic initiative were orchestrated as a coordinated effort.",
          content1:
            "They turned to QUANTUM WORLD for a better prospects and who could meet their aggressive goals and compete with its complex structure. The company which can translate the client’s vision into a actionable plan, identify the right resources to involve, coordinate all stakeholders toward the common goal and proceed towards the goal. Just after few time instance, QUANTUM WORLD plays a key role in unifying the program, the architectural structure, minimizing confusion, improving communications among business units and senior leadership, building an awareness among team members on the strategic implications of the program, and establishing and managing the schedule to ensure that strategic milestones were being met.",
        },
        {
          head: "Retail",
          image: "http://quantumworld.in/wp-content/uploads/2016/11/retail.jpg",
          content:
            "QUANTUM WORLD practice is maturing in providing consulting to global retail customers in the areas of Enterprise application service with offerings like Global ERP, Application Maintenance and Support, Digital Transformation, E-Commerce & Omni Channel, Enterprise Performance Management and Analytics, Enterprise Asset Management and Human Capital Management.",
        },
        {
          head: "IT / Technologies",
          image: "http://quantumworld.in/wp-content/uploads/2016/11/15.jpg",
          content:
            "We at QUANTUM WORLD having a strong senior management commitment for the IT / Technology initiative, members of the organization's IT team adopts the best improvement plan as recommended and began executing them with guidance and support provided by senior consultants from QUANTUM WORLD.",
          content1:
            " We serve IT / Technologies industries in providing them support for personnel in different sector and trade. We support all technical as well as staffing needs in all major segments of the IT / Technologies industry, which includes Core Banking, Corporate banking, Wholesale Banking, Retail Banking, Payment Gateways, Mutual Funds, Accounting & Billing, Insurance and many more.",
        },
        {
          head: "Transportation and logistics",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/transport.png",
          content:
            "Growing competition and globalized operations make it necessary for logistics service providers (LSPs) to effectively collaborate with partners across the value chain, monitor processes end-to-end and adopt preventive strategies over the more traditional reactive approach to sustain profitability. To drive this, LSPs need to process large volumes of transaction data in real time to gain visibility into the supply chain, improve strategic decision making and deliver more efficient customer service.",
          content1:
            "We as QUANTUM WORLD offers a wide range of solutions that help LSPs improve customer and vendor relationships, realize efficiencies, and utilize assets more productively. From enhancing customer and vendor management to optimizing managed transportation to driving digital transformation, our solutions empower LSPs to improve service delivery and drive customer centricity.",
        },
        {
          head: "Life Sciences",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/lifescience.jpg",
          content:
            "QUANTUM WORLD Life Sciences Solutions and Services help Pharmaceutical, Biotech, Medical Devices and Diagnostics companies to accelerate drug discovery, advance clinical trial efficiencies, accentuate manufacturing productivity and amplify sales and marketing effectiveness.",
          content1:
            "With over two decades of experience in working with global life sciences companies, in diverse geographies, QUANTUM WORLD your trusted partner and advisor, will help you in your transformation journey, through its people, platforms and products / services across the value chain.",
        },
        {
          head: "Automotive",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/automotive1.jpg",
          content:
            "The QUANTUM WORLD provides true value stream optimization - from core & embedded engineering skills to product lifecycle management (PLM), manufacturing execution systems (MES), supply chain management (SCM) and dealer management systems (DMS).",
          content1:
            " Our automotive clients have frequently expressed the desire to be agile, aligning their business operations with the market needs. We can support you with comprehensive value chain enablement strategy, driven by customer pull. Our right sourcing capabilities across each value chain element have earned the loyalty of the industry leaders. Our services include Value Chain Assessment and Lean Design, Total Outsourcing for Application Management and System Integration Services. To help our clients derive value from such engagements we offer LEAN Consulting, Automotive Business Solutions and Enterprise Transformation services.",
        },
      ],
    };
  },
};
</script>

<style>
.cardIndustry {
  height: 400px;
}
</style>
