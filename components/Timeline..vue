<template>
  <v-timeline>
    <v-timeline-item
      v-for="dataItem in timeLineData"
      :key="dataItem.year"
      :color="dataItem.color"
      small
    >
      <template v-slot:opposite>
        <v-img
          :class="`headline font-weight-bold ${dataItem.color}--text`"
          :src="dataItem.image"
          height="180"
          contain
        ></v-img>
      </template>
      <div class="py-4">
        <h2 :class="`headline font-weight-light mb-4 ${dataItem.color}--text`">
          {{ dataItem.title }}
        </h2>
        <div>
          {{ dataItem.textContaint }}
        </div>
      </div>
    </v-timeline-item>
  </v-timeline>
</template>

<script>
export default {
  data: () => ({
    timeLineData: [
      {
        title: "Setup and support on day one",
        color: "cyan",
        image:
          "https://www.uber-assets.com/image/upload/f_auto,q_auto:eco,c_fill,w_360,h_203/v1573763089/assets/30/f00a50-9092-4f31-a627-e5637bbacbce/original/Setup-and-support.png",
        textContaint:
          "With a starter kit and free food photo shoot, plus our order and menu management software, we get you looking great in the Uber Eats app and ready to satisfy customers.",
      },
      {
        title: "Manage orders with efficient tools",
        color: "green",
        image:
          "https://www.uber-assets.com/image/upload/f_auto,q_auto:eco,c_fill,w_360,h_203/v1573683122/assets/2c/04062b-7469-477f-9c93-b21437b33668/original/ManageOrdersWithEase.png",
        textContaint:
          "See how you can boost your front-of-house workflow with our Restaurant Dashboard. Once you’re a partner, we’ll help you integrate orders from customers using the Uber Eats app with your existing POS to keep the whole staff in sync.",
      },
      {
        title: "Deliver the way you want",
        color: "pink",
        image:
          "https://www.uber-assets.com/image/upload/f_auto,q_auto:eco,c_fill,w_360,h_203/v1573683154/assets/66/6e7309-df29-401a-a1ba-16d65daf28de/original/Deliveryonyourownterms.png",
        textContaint:
          "Offer reliable delivery to your customers with the flexibility you need. Connect with delivery people using the Uber platform, use your own delivery staff, or try a combination",
      },
      {
        title: "Expand your marketing",
        color: "amber",
        image:
          "https://www.uber-assets.com/image/upload/f_auto,q_auto:eco,c_fill,w_360,h_203/v1573683185/assets/21/d011b9-cf61-4cc9-ae67-894ae8de6afe/original/ExpandYourMarketing.png",
        textContaint:
          "Run promotions, get a boost from Uber’s marketing reach—and enjoy more big opportunities to reach new customers in your city.",
      },
      {
        title: "Get data that matters",
        color: "orange",
        image:
          "https://www.uber-assets.com/image/upload/f_auto,q_auto:eco,c_fill,w_360,h_203/v1573683217/assets/62/9e475c-e3f9-4d38-881f-387e899935fd/original/GetDataThatMatters.png",
        textContaint:
          "Bring your performance into focus with insightful, actionable analytics. See key details like sales and customer feedback, with the context you need to act.",
      },
    ],
  }),
};
</script>