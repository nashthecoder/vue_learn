<script>
import { Radar } from "vue-chartjs";

export default {
  extends: Radar,
  data() {
    return {
      chartData: {
        labels: ["Netherlands", "Spain", "Portugal", "Estonia"],
        datasets: [
          {
            borderWidth: 1,
            borderColor: [
              "rgba(255,99,132,1)"
            ],
            backgroundColor: [
              "rgba(255, 99, 132, 0.2)"
            ],
            data: [200, 1400, 800, 1000]
          }
        ]
      },
      options: {
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
