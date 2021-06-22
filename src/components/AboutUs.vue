<template>
  <div class="flex-center column">
    <div class="q-mt-xl text-h2 text-weight-regular">About Quantum World</div>
    <q-card class="q-mt-xl shadow-12">
      <q-tab-panels v-model="tab" animated class="aboutClass">
        <q-tab-panel name="about">
          <div class="text-h6 q-pa-lg">
            Quantum World is a leading consulting and services company in India
            (specially in Noida & Lucknow) and provide a manpower solution at
            multinational companies. Quantum World offers wide gamut of
            consulting solutions customized to specific needs. We as one of the
            leading service provider, provides effective business solutions in
            IT Consulting & Staff Augmentation, Project Management, Product
            Engineering and Business Process Outsourcing Services. Our Staffing
            division places top Technology Professionals in contract,
            contract-to-hire, direct hire and SOW / Statement of Work based
            positions with industry leaders and innovative start-ups that are
            developing the next generation of technology solutions. We have been
            recognized as one of the Largest and Fastest Growing Staffing Firms
            as ranked by Staffing Industry Analysts.
          </div>
        </q-tab-panel>

        <q-tab-panel name="vision">
          <div class="text-h6 q-pa-lg">
            To structure how India pays through innovation, the power of
            seamless connectivity and the ability of cost-effective solutions
            that mutually transports business systems to incredible new horizons
            in performance, profit and customer satisfaction. Our onsite and
            offshore development model allows us to leverage local competencies
            to offer global competitiveness to our clients ensuring high
            quality, on time delivery, at significantly reduced costs. We use a
            low-risk Model to accelerate schedules with a high degree of time
            and cost predictability.We provide solutions for a dynamic
            environment where business and technology strategies converge. We
            provides consulting and IT services to clients globally - as
            partners to conceptualize and realize technology driven business
            transformation initiatives.
          </div>
        </q-tab-panel>

        <q-tab-panel name="mission">
          <div class="text-h6 q-pa-lg">
            To eternally adapt, create & innovate to deliver an open payments
            processing platform that seamlessly integrates with banks, business
            systems and consumers. Quantum tech usa are built on state-of-art
            infrastructure and technology with one key ambition, to drive value
            for your business and for your customers.Our approach focuses on new
            ways of business combining IT innovation and adoption while also
            leveraging an organization's current IT assets. As a diverse
            end-to-end IT solutions provider, the company offers a range of
            expertise aimed at helping customers re-engineer and re-invent their
            businesses to compete successfully in an ever-changing marketplace.
            With a world-class infrastructure and a global network, Quantum
            World offers a wide array of solutions for a range of key verticals
            and horizontals; starting from the strategy consulting right through
            to implementing IT solutions for clients. As a certified MBE,
            QUANTUM WORLD supports and promotes supplier and workforce
            diversity, and has placed over many Technology Professionals.
          </div>
        </q-tab-panel>
      </q-tab-panels>
      <q-separator />
      <q-tabs
        v-model="tab"
        dense
        class="bg-grey-3"
        align="justify"
        narrow-indicator
      >
        <q-tab name="about" label="About Us" />
        <q-tab name="vision" label="Vision" />
        <q-tab name="mission" label="Mission" />
      </q-tabs>
    </q-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tab: "about",
    };
  },
};
</script>

<style>
.aboutClass {
  background: linear-gradient(
    0deg,
    rgba(108, 204, 207, 1) 0%,
    rgba(253, 254, 255, 1) 21%,
    rgba(169, 199, 235, 1) 85%,
    rgba(69, 134, 211, 1) 100%
  );
}
</style>
