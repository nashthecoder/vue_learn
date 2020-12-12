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
            label: "Bar Chart",
            borderWidth: 1,
            backgroundColor: [
              "rgba(255, 99, 132, 0.2)",
              "rgba(54, 162, 235, 0.2)",
              "rgba(255, 206, 86, 0.2)",
              "rgba(75, 192, 192, 0.2)",
              "rgba(153, 102, 255, 0.2)",
              "rgba(255, 159, 64, 0.2)",
              "rgba(255, 99, 132, 0.2)",
              "rgba(54, 162, 235, 0.2)",
              "rgba(255, 206, 86, 0.2)",
              "rgba(75, 192, 192, 0.2)",
              "rgba(153, 102, 255, 0.2)",
              "rgba(255, 159, 64, 0.2)"
            ],
            borderColor: [
              "rgba(255,99,132,1)",
              "rgba(54, 162, 235, 1)",
              "rgba(255, 206, 86, 1)",
              "rgba(75, 192, 192, 1)",
              "rgba(153, 102, 255, 1)",
              "rgba(255, 159, 64, 1)",
              "rgba(255,99,132,1)",
              "rgba(54, 162, 235, 1)",
              "rgba(255, 206, 86, 1)",
              "rgba(75, 192, 192, 1)",
              "rgba(153, 102, 255, 1)",
              "rgba(255, 159, 64, 1)"
            ],
            pointerBorderColor: "#2554FF",
            data: [12, 19, 7, 5, 2, 13, 20, 3, 5, 6, 2, 4]
          }
        ]
      },

      options: {
        scales: {
          yAxes: [
            {
              ticks: {
                beginAtZero: true
              },
              grindlines: {
                display: true
              }
            }
          ],
          xAxes: [
            {
              grindlines: {
                display: false
              }
            }
          ]
        },
        legend: {
          display: true
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
