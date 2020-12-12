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
            pointBackgroundColor: ["green",
            "blue",
            "yellow",
            "orange",
            "purple"
                ],
            data: [600, 1150, 342, 6050, 2522, 3241, 1259, 157, 1545, 9841],
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
              gridLines: {
                display: true
              }
            }
          ],
          xAxes: [
            {
              gridLines: {
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
