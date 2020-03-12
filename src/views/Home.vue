<template>
  <b-container>
    <b-row align-v="center">
      <ajob
        v-for="data in displayDatas"
        :key="data.id"
        :name="data.name"
        img-src="https://picsum.photos/seed/picsum/200/300"
      ></ajob>
    </b-row>
    <br />
    <b-pagination
      align="center"
      v-model="currentPage"
      :total-rows="rows"
      :per-page="perPage"
      first-text="First"
      prev-text="Prev"
      next-text="Next"
      last-text="Last"
      @input="paginate(currentPage)"
    ></b-pagination>
    <br />
  </b-container>
</template>
<script>
// @ is an alias to /src
import job from "@/components/job.vue";

export default {
  name: "Home",
  components: { ajob: job },
  mounted() {
    this.fetchData();
  },
  data() {
    return {
      datas: [],
      displayDatas: [],
      currentPage: 1,
      rows: 1,
      perPage: 3
    };
  },
  methods: {
    async fetchData() {
      const res = await fetch("datas.json");
      const val = await res.json();
      this.datas = val;
      this.displayDatas = val.slice(0, 3);
      this.rows = this.datas.length;
      console.log(val);
    },
    paginate(currentPage) {
      const start = (currentPage - 1) * this.perPage;
      this.displayDatas = this.datas.slice(start, start + 3);
    }
  }
};
</script>
