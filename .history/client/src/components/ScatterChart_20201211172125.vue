<script>
import { Scatter } from "vue-chartjs";

export default {
  extends: Scatter,
  data() {
    return {
      chartData: {
        labels: [
          "Mombasa",
          "Kilifi",
          "Diani",
          "Amsterdam",
          "Barcelona",
          "Porto",
          "Accra",
          "Lagos",
          "Dakar",
          "Rotterdam"
        ],

        datasets: [
          {
            label: "Scatter Chart",
            pointBackgroundColor: [
              "green",
              "blue",
              "yellow",
              "orange",
              "purple"
            ],
            data: [
              { x: 0, y: 10 },
              { x: 2, y: 8 },
              { x: 4, y: 10 },
              { x: 7, y: 5 },
              { x: -2, y: 0 }
            ]
          }
        ]
      },
      options: {
        legend: {
          display: false
        },
        xAxes: [
          {
            type: "linear",
            position: "bottom"
          }
        ],
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
