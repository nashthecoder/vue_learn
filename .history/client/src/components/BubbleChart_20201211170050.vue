<script>
import { Bubble } from "vue-chartjs";

export default {
  extends: Bubble,
  data() {
    return {
      chartData: {
        labels: [
          "J 2020",
          "F 2020",
          "M 2020",
          "A 2020",
          "M 2020",
          "J 2020",
          "J 2020",
          "A 2020",
          "S 2020",
          "O 2020",
          "N 2020",
          "D 2020"
        ],
        datasets: [
          {
            label: "My colors",
            borderWidth: 1,
            backgroundColor: [
              "rgba(255, 99, 132, 0.2)",
              "rgba(54, 162, 235, 0.2)",
              "rgba(255, 206, 86, 0.2)",
              "rgba(75, 192, 192, 0.2)"
            ],
            borderColor: ["#fff"],
            pointerBorderColor: "#2554FF",
            data: [{x: 5, y:10, r:10}, {x: 15, y:3, r:15}, {x: 7, y:15, r:30}, {x: 25, y:5, r:10}]
          }
        ]
      },

      options: {
        legend: {
          display: false
        },
        responsive: true,
        maintainAspectRatio: false
      }
    };
  },
  mounted() {
    this.renderChart(this.chartData, this.options);
  }
};
</script>
