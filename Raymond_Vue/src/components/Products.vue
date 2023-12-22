<script>
import Product from "./Product.vue";

export default {
  components: {
    Product,
  },
  data() {
    return {
      products: [
        {
          id: "1",
          imageUrl: "https://loremflickr.com/g/320/600/paris?random=1",
          productName: "Location 1",
          releasedDate: "May 13, 2023",
          description: "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat.",
          rating: 4,
        },
        {
          id: "2",
          imageUrl: "https://loremflickr.com/320/600/brazil,rio?random=2",
          productName: "Location 2",
          releasedDate: "October 31, 2023",
          description: "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat.",
          rating: 2,
        },
        {
          id: "3",
          imageUrl: "https://loremflickr.com/g/320/600/paris?random=3",
          productName: "Location 3",
          releasedDate: "May 24, 2023",
          description: "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat.",
          rating: 5,
        },
        {
          id: "4",
          imageUrl: "https://loremflickr.com/g/320/600/paris?random=4",
          productName: "Location 4",
          releasedDate: "April 1, 2023",
          description: "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat.",
          rating: 5,
        },
        {
          id: "5",
          imageUrl: "https://loremflickr.com/320/600/brazil,rio?random=5",
          productName: "Location 5",
          releasedDate: "February 28, 2023",
          description: "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat.",
          rating: 5,
        },
      ],
    };
  },
};
</script>
<template>
  <div v-for="product in products" :key="product.id">
    <Product :data="product" />
  </div>
</template>