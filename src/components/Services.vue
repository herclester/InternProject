<template>
  <div class="row">
    <q-list v-for="card in cardss" :key="card.head" class="q-pa-lg col-4">
      <q-item>
        <q-item-section>
          <q-card class="shadow-12 text-center cardServices1">
            <q-card-section class="text-white text-h4">
              {{ card.head }}
            </q-card-section>
            <q-card-section style="height: 300px">
              <q-img :src="card.image" width="50%" />
            </q-card-section>
            <q-card-section class="text-white text-subtitle1">
              {{ card.content1 }}
            </q-card-section>
            <q-card-section
              class="text-subtitle1 text-white"
              v-if="card.content2"
            >
              {{ card.content2 }}
            </q-card-section>
          </q-card>
        </q-item-section>
      </q-item>
    </q-list>
    <q-list v-for="card in cardss2" :key="card.head" class="q-pa-lg col-4">
      <q-item>
        <q-item-section>
          <q-card class="shadow-12 text-center cardServices2">
            <q-card-section class="text-white text-h4">
              {{ card.head }}
            </q-card-section>
            <q-card-section style="height: 250px">
              <q-img :src="card.image" width="50%" />
            </q-card-section>
            <q-card-section class="text-subtitle1 text-white">
              {{ card.content1 }}
            </q-card-section>
            <q-card-section
              class="text-subtitle1 text-white"
              v-if="card.content2"
            >
              {{ card.content2 }}
            </q-card-section>
          </q-card>
        </q-item-section>
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
          head: "Application Development",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/ApplicationDevelopment-1.jpg",
          content1:
            "The value of a prototype is in the education it gives you, not in the code itself.",
          content2:
            "We as QUANTUM WORLD offers one of our best service i.e. Application Development and Maintenance Services. Under this service we offer our clients the full scope of services - development, implementation on newly created or an ongoing management. Our process model offers our clients a robust and industrialized approach for both new and existing applications across a variety of platforms and technologies.",
        },
        {
          head: "Manpower Outsourcing",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/teaserbox_4097441546.jpg",
          content1:
            "From Multinational Conglomerates to MSMEs, every business entity understands the advantages of outsourcing. With ever increasing business demands companies want to stay focused on their core business activity and outsource support services to save time & energy. To remain competitive they want to reduce costs and enhance employee productivity. Manpower Outsourcing achieves these twin objectives.",
          content2:
            "Quantam World is the pioneer of Engineering Manpower Outsourcing services in India. We provide tailor-made solutions depending on client needs. Be it complete project based requirement on Turnkey basis, short term requirement for Project Peak Periods, expected / unexpected load or towards the end of project or requirement of specialized manpower or simply the need for third party pay roll services, we have solutions for all",
        },
        {
          head: "ITES Staffing",
          image:
            "http://quantumworld.in/wp-content/uploads/2015/06/image_6.jpg",
          content1:
            "Quantum World Tech is a pioneer in rendering HR Solutions across the country. It is a combined venture of leading and experienced HR Professionals & Masters. The company laid its roots from basics of HR Management, thereby bringing a unique approach to cater the requirements of our Clients.",
          content2:
            "Our rigorous screening procedure ensures quality output within specific time frames. You can completely rely on us to handle even the most critical requirements in shortest possible time, which is of paramount importance in these evolving times. We keep abreast of the rapid developments that take place in the corporate arena and constantly review and upgrade ourselves to tackle these developments in the most effective manner.",
        },
        {
          head: "Deputation/Manpower Outsourcing",
          image: "http://quantumworld.in/wp-content/uploads/2016/11/15-4.jpg",
          content1:
            "Each and every business entity comprehends the benefits of Deputation/Manpower Outsourcing. With ever mounting business demands companies want to stay focused on their core business movement and outsource support services to save energy &time. To remain spirited they want to lessen costs and improve employee efficiency. Manpower Outsourcing attains these twin objectives.",
          content2:
            "Our company is the pioneer of international recruitment and selection services in India. We provide customized solutions depending on client demands. Be it absolute project based demands on turnkey basis, short term demands for project peak periods, expected / unexpected load or towards the end of project of specialized manpower or merely the requirement for third party pay roll services, we encompass solutions for all.",
        },
        {
          head: "International Job Placement Consultancy",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/84770f_727d873ba990ce1d7c594b88d300cb63.jpg_srz_1280_1092_85_22_0.50_1.20_0.00_jpg_srz.jpg",
          content1:
            "We are a dependable International Job Placement Consultancy providing you with best overseas placement consultancy services and manpower consultancy services matching the industrial requirements for professional manpower. Our process-driven firm helps clients in employing trained professionals for diverse industries.Our team of professionals has made a mark as one of the most renowned job recruitment consultants. ",
          content2:
            "Our proficiency coupled with precise industry expertise gives us the strength to meet the most challenging of assignments in the specific time period. It is our responsibility to comprehend every employer's particular demands that is why we work in close harmonization with our clients. ",
        },
        {
          head: "International Manpower Recruitment",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/manpower-2.png",
          content1:
            "The International Manpower Recruitment Services concentrate on international placement. It encompasses a pool of qualified and trained candidates ranging from unskilled labors to top management level across industry verticals. Here we are primarily concerned in providing human resource from India to diverse parts of the globe plying talent to varied industries like - infrastructure. it, retail, oil & gas, power, hospitality and banking & finance.",
          content2:
            "Keeping in mind the contemplations like industry-specific skills and the location, we select the best candidates. In addition to this, the services offered by us also acts as the backend hold up for its diverse offices in international markets, thus making sure that we deliver right personnel solutions as per the demands of clients at lowest costs. ",
        },
      ],
      cardss2: [
        {
          head: "Assessment and Recruitment",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/assessment-and-recruitment-1.jpg",
          content1:
            "Our proven recruitment, assessment and selection methods ensure that we identify the talent with the necessary skills and personal attributes that will add value to your organization.",
        },
        {
          head: "HR Consultancy",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/Img_573b25f245219slide_hr_consultancy.jpg",
          content1:
            "By associating with our HR Consultancy to handle your HR Outsourcing or contracting for India administration, you can leverage the modernized efficiencies and the buying authority of our huge organization, making noteworthy savings in both time and costs. We can develop custom-made HR outsourcing services for you based on the kind of personnel you have and the precise needs of your business. You deserve an associate that can provide you with the liberty to focus on developing your business every day.",
        },
        {
          head: "Career Management",
          image: "http://quantumworld.in/wp-content/uploads/2016/11/blog.jpg",
          content1:
            "We help you respond to changing marketing conditions and emerging business opportunities by strategically mobilizing and sizing your workforce to meet the needs of your business, minimize turnover and maintain productivity.",
        },
        {
          head: "Outsourcing",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/outsource_finger.jpg",
          content1:
            "We provide innovative outsourcing solutions across a wide range of disciplines. The world’s leading companies turn to us for Talent Based Outsourcing, Recruitment Process Outsourcing, Managed Service Provider Solutions and Borderless Talent Solutions.",
        },
        {
          head: "Workforce Consulting",
          image: "http://quantumworld.in/wp-content/uploads/2016/11/15-5.jpg",
          content1:
            "We align your workforce strategy with your business strategy, improving work models and increasing the agility and the competiveness of your workforce and your entire organization.",
        },
        {
          head: "Professional Development",
          image:
            "http://quantumworld.in/wp-content/uploads/2016/11/Professional-Development-Picture.png",
          content1:
            "We offer a full array of resources, from online training for a small-business staff to customized programs for businesses of all sizes, including many of the Fortune 500 companies, to ensure that your talent has the skills and knowledge needed to drive your business forward.",
        },
      ],
    };
  },
};
</script>

<style>
.cardServices1 {
  height: 950px;
  background: radial-gradient(
    circle,
    rgba(108, 204, 207, 1) 0%,
    rgba(34, 83, 143, 1) 91%
  );
}
.cardServices2 {
  height: 625px;
  background: radial-gradient(
    circle,
    rgba(108, 204, 207, 1) 0%,
    rgba(34, 83, 143, 1) 91%
  );
}
</style>
